---
layout: page
title: P2O
description: AI-driven dashboard for water utilities
img: assets/img/P2O.png
importance: 3
category: work
---

<h2>Prediction in Water Distribution Systems - P<sub>2</sub>O</h2>

<p>This section focuses on the Multivariate Multi-step LSTM (MM-LSTM) and other AI models for tunnel water level prediction and optimization. A schematic diagram of the methodology used for this module is shown in Figure 1. This module includes five main components: Data Preprocessing, Exploratory Data Analysis (EDA), Model Development, Hyperparameter Tuning, and Model Evaluation & Selection. Details of each component are discussed below.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/Figure_3.pdf" alt="Schematic Diagram of Methodology Used for Tunnel Water Level Prediction" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 1: Schematic Diagram of Methodology Used for Tunnel Water Level Prediction</em> (<a href="https://doi.org/10.1016/j.compenvurbsys.2023">Kulkarni et al., 2023</a>)</p>
        </div>
    </div>
</div>

<h3>Data Preprocessing for Tunnel Wastewater Level Prediction</h3>

<p>The data used for this work come from an actual water distribution system (WDS) with 243 columns in each file. Initially, the Not Available (NA) sensor readings were handled by removing them from the dataset, resulting in 42 columns after preprocessing. The dataset contained 367,943 rows after eliminating NA values, with preprocessing including techniques like Principal Component Analysis (PCA) and downsampling to reduce data redundancy and improve model performance.</p>

<p>PCA was used to handle collinearity in the data, creating a dataset with uncorrelated features. Downsampling, performed by selecting observations at 30-minute intervals, resulted in two versions of the data at the end of preprocessing, one based on PCA and the other on the raw downsampled data.</p>

<h3>Multivariate Multi-step LSTM Model Development</h3>

<p>The Multivariate Multi-step LSTM (MM-LSTM) model is developed using a Long Short-Term Memory (LSTM) architecture for time-series forecasting. This model is designed to take multiple input features to predict multi-step outputs, such as future tunnel water levels. The goal is to accurately predict water levels while prioritizing overflow incidents, as these are critical events in water management.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/MM-LSTM.png" alt="Water Level Forecasting LSTM Architecture" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 2: Water Level Forecasting LSTM Architecture</em></p>
        </div>
    </div>
</div>

<p>Given the importance of overflow events, the Huber loss function (Equation 1) was selected as the objective function to handle outliers caused by extreme weather conditions and overflow situations. The training data are sequences of 24, 48, and 72-hour intervals, which are used to predict 2 to 6-hour multi-step forecasts. Adam optimizer is used for training, and the model's performance is evaluated on a test set comprising 30% of the original data.</p>

<pre>
<code>
\[
L(y, f(x)) = \begin{cases}
    \frac{1}{2}(y - f(x))^2 & \text{if } |y - f(x)| \leq \delta \\
    \delta(|y - f(x)| - \frac{1}{2}\delta) & \text{if } |y - f(x)| > \delta
\end{cases}
\]
</code>
</pre>

<p>After training, the model outputs are transformed back to the original scale for comparison with actual water levels. The key focus is on detecting peak water levels, especially during overflow conditions, defined as water levels exceeding -47 feet.</p>

<h3>Model Optimization and Explainability</h3>

<p>The MM-LSTM model is optimized using the Huber loss function, which is a robust alternative to Mean Squared Error (MSE) and less sensitive to outliers. The Huber loss function adjusts dynamically between MSE and Mean Absolute Error (MAE), providing a balance between outlier resistance and smooth optimization.</p>

<pre>
<code>
\[
L(y, f(x)) = \begin{cases}
    \frac{1}{2}(y - f(x))^2 & \text{if } |y - f(x)| \leq \delta \\
    \delta(|y - f(x)| - \frac{1}{2}\delta) & \text{if } |y - f(x)| > \delta
\end{cases}
\]
\]
</code>
</pre>

<p>To improve the interpretability of the deep learning model, SHAP (Shapley Additive Explanations) values are used to estimate feature importance. SHAP provides insights into the contribution of each feature to the model's output by applying a game-theory-based approach to calculate contribution scores for each prediction. By analyzing SHAP values, operators can gain a better understanding of critical features influencing tunnel water levels, optimizing the operational decision-making process.</p>

<h4>Algorithm: Multivariate Multistep LSTM with Huber Loss for Tunnel Water Level Forecasting and Anomaly Detection</h4>

<pre>
<code>
\begin{algorithm}[ht]
\resizebox{\linewidth}{!}{
\begin{minipage}{\linewidth}
\caption{Multivariate Multistep LSTM with Huber Loss for Tunnel Water Level Forecasting with Anomaly Detection}
\label{algo:LSTM-huber-anomaly-detection}
\begin{algorithmic}[1]
\STATE \textbf{Input:} Multivariate time series data $X$, LSTM model parameters, prediction horizon $H$, anomaly threshold $T$
\STATE \textbf{Output:} Forecasted water levels and anomaly labels

\STATE Split $X$ into training ($X_{\text{train}}$) and testing ($X_{\text{test}}$) datasets

\STATE Train the LSTM model on the training dataset using Huber loss
\STATE Initialize model parameters and hyperparameters: $\Theta = \{\theta_1, \theta_2, \ldots, \theta_n\}$

\STATE \textbf{Training Phase:}
\FOR{$i$ in $\text{number of epochs}$}
    \FOR{$j$ in $\text{mini-batches}$ of training data}
        \STATE Forward pass: Encode and decode the data, $\hat{X} = \text{LSTM}(\text{Encode}(X_{\text{batch}}, \Theta), \Theta)$
        \STATE Calculate Huber loss for $H$-step ahead predictions: $L_{\text{Huber}} = \text{HuberLoss}(X_{\text{batch}}, \hat{X}, \delta)$
        \STATE Backpropagation: Update model weights to minimize Huber loss, $\Theta \leftarrow \Theta - \eta \nabla L_{\text{Huber}}$
    \ENDFOR
\ENDFOR

\STATE \textbf{Testing Phase:}
\FOR{$k$ in $\text{mini-batches}$ of testing data}
    \STATE Forward pass: Encode and decode the data, $\hat{X} = \text{LSTM}(\text{Encode}(X_{\text{batch}}, \Theta), \Theta)$
    \STATE Calculate Huber loss for $H$-step ahead predictions for each sample: $L_{\text{sample}} = \text{HuberLoss}(X_{\text{batch}}, \hat{X}, \delta)$
    \IF{$L_{\text{sample}} > T$}
        \STATE Mark as an anomaly
    \ELSE
        \STATE Mark as normal
    \ENDIF
\ENDFOR

\RETURN Forecasted water levels and anomaly labels
\end{algorithmic}
\end{minipage}
}
\end{algorithm}
\end{code>
</pre>

<p>The use of SHAP values helps to explain the model's predictions by highlighting the contribution of different features. For example, this approach enables water utility operators to make informed decisions on when to activate pumps to prevent tunnel overflow based on critical feature importance.</p>
