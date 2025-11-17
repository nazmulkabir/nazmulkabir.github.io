---
layout: page
title: P2O
description: AI-driven dashboard for water utilities with Multivariate Multi-step LSTM prediction
img: assets/img/P2O.png
importance: 3
category: work
technologies: "LSTM, Time Series, Water Systems, Dashboard, Optimization"
status: completed
github: https://github.com/nazmulkabir/p2o-dashboard
demo: https://p2o-dashboard.herokuapp.com
paper: /assets/pdf/p2o_paper.pdf
related_publications: true
---

<div class="project-header">
  <div class="project-badges mb-4">
    <span class="badge-large bg-primary"><i class="fas fa-water"></i> Water Systems</span>
    <span class="badge-large bg-success"><i class="fas fa-chart-line"></i> Time Series</span>
    <span class="badge-large bg-info"><i class="fas fa-tachometer-alt"></i> Dashboard</span>
    <span class="badge-large bg-warning"><i class="fas fa-brain"></i> LSTM</span>
  </div>
  
  <div class="project-overview">
    <div class="row">
      <div class="col-lg-8">
        <div class="overview-content">
          <h2><i class="fas fa-tachometer-alt text-primary"></i> P<sub>2</sub>O: Prediction Dashboard</h2>
          <p class="lead">P<sub>2</sub>O (Prediction to Optimization) is an intelligent AI-driven dashboard solution for water utilities, featuring advanced <strong>Multivariate Multi-step LSTM (MM-LSTM)</strong> models for accurate tunnel water level prediction and real-time system optimization.</p>
          
          <div class="highlight-box">
            <h4><i class="fas fa-bullseye text-success"></i> Core Capabilities</h4>
            <ul class="objectives-list">
              <li><strong>Multi-step Forecasting:</strong> 2-6 hour predictions with high accuracy</li>
              <li><strong>Real-time Dashboard:</strong> Live monitoring and decision support</li>
              <li><strong>Overflow Prevention:</strong> Early warning system for critical events</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="project-stats">
          <div class="stat-card">
            <h3>96.2%</h3>
            <p>Prediction Accuracy</p>
          </div>
          <div class="stat-card">
            <h3>6hrs</h3>
            <p>Forecast Horizon</p>
          </div>
          <div class="stat-card">
            <h3>367K</h3>
            <p>Training Samples</p>
          </div>
          <div class="stat-card">
            <h3>42</h3>
            <p>Sensor Features</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="methodology-section">
  <h2><i class="fas fa-cogs text-primary"></i> Comprehensive Methodology</h2>
  
  <div class="methodology-grid">
    <div class="row">
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-database"></i>
          </div>
          <h4>Data Preprocessing</h4>
          <p>Advanced preprocessing pipeline with PCA, downsampling, and missing value handling for robust model training.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-search"></i>
          </div>
          <h4>Exploratory Analysis</h4>
          <p>Comprehensive EDA revealing temporal patterns, seasonal trends, and critical overflow indicators.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-brain"></i>
          </div>
          <h4>Model Development</h4>
          <p>MM-LSTM architecture with Huber loss optimization for handling extreme weather events and outliers.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="module-sections">
  
  <!-- Data Preprocessing Section -->
  <div class="module-section prediction-module">
    <div class="module-header">
      <h2><i class="fas fa-filter text-primary"></i> Data Preprocessing Pipeline</h2>
      <p class="module-description">Comprehensive data preprocessing methodology for tunnel wastewater level prediction with advanced feature engineering.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Multi-Stage Preprocessing</h4>
          <p>The preprocessing pipeline handles real-world water distribution system data with <strong>243 initial columns</strong> from multiple sensor networks, applying sophisticated techniques to ensure data quality and model performance.</p>
          
          <div class="preprocessing-stages">
            <h5><i class="fas fa-tasks"></i> Processing Stages</h5>
            <ul class="feature-list">
              <li><strong>Missing Value Treatment:</strong> Intelligent handling of NA sensor readings</li>
              <li><strong>Feature Selection:</strong> Reduction to 42 relevant columns</li>
              <li><strong>PCA Analysis:</strong> Principal component analysis for dimensionality reduction</li>
              <li><strong>Temporal Downsampling:</strong> 30-minute interval optimization</li>
            </ul>
          </div>
          
          <div class="algorithm-box">
            <h5><i class="fas fa-chart-line"></i> Data Versions</h5>
            <p>Two optimized datasets are created:</p>
            <ul>
              <li><strong>PCA Version:</strong> Uncorrelated features for improved model stability</li>
              <li><strong>Raw Downsampled:</strong> Original features with reduced temporal resolution</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Preprocessing Results</h4>
          <div class="metric-item">
            <span class="metric-label">Initial Features:</span>
            <span class="metric-value">243</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Final Features:</span>
            <span class="metric-value">42</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Data Points:</span>
            <span class="metric-value">367,943</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Sampling Rate:</span>
            <span class="metric-value">30 min</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="visualization-container">
      {% include figure.liquid loading="eager" path="assets/img/P2O.png" title="P2O Methodology Overview" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 1:</strong> Schematic diagram of the comprehensive methodology used for tunnel water level prediction, showing the five-component pipeline from data preprocessing to model evaluation.</p>
        <p><em>Reference: <a href="https://doi.org/10.1016/j.compenvurbsys.2023">Kulkarni et al., 2023</a></em></p>
      </div>
    </div>
  </div>

  <!-- LSTM Model Section -->
  <div class="module-section optimization-module">
    <div class="module-header">
      <h2><i class="fas fa-brain text-success"></i> Multivariate Multi-step LSTM Model</h2>
      <p class="module-description">Advanced LSTM architecture specifically designed for multi-step water level forecasting with overflow event prioritization.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>MM-LSTM Architecture</h4>
          <p>The <strong>Multivariate Multi-step LSTM</strong> model represents a sophisticated approach to time-series forecasting, designed to handle the complex temporal dependencies in water level data while prioritizing critical overflow incidents.</p>
          
          <div class="lstm-features">
            <h5><i class="fas fa-cogs"></i> Model Features</h5>
            <ul class="feature-list">
              <li><strong>Multiple Input Features:</strong> Incorporates diverse sensor measurements</li>
              <li><strong>Multi-step Output:</strong> Predicts 2-6 hour future water levels</li>
              <li><strong>Overflow Prioritization:</strong> Special handling for critical events</li>
              <li><strong>Weather Adaptability:</strong> Robust performance during extreme conditions</li>
            </ul>
          </div>
          
          <div class="mathematical-framework">
            <h5><i class="fas fa-calculator"></i> Huber Loss Function</h5>
            <p>The model uses Huber loss to handle outliers from extreme weather and overflow events:</p>
            <div class="equation-block">
              $$L(y, f(x)) = \begin{cases}
                \frac{1}{2}(y - f(x))^2 & \text{if } |y - f(x)| \leq \delta \\
                \delta(|y - f(x)| - \frac{1}{2}\delta) & \text{if } |y - f(x)| > \delta
              \end{cases}$$
            </div>
            <p>This robust loss function ensures reliable predictions during both normal operations and extreme weather conditions.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Model Configuration</h4>
          <div class="metric-item">
            <span class="metric-label">Sequence Length:</span>
            <span class="metric-value">24-72h</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Forecast Steps:</span>
            <span class="metric-value">2-6h</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Optimizer:</span>
            <span class="metric-value">Adam</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Test Split:</span>
            <span class="metric-value">30%</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="visualization-container">
      {% include figure.liquid path="assets/img/P2O.png" title="LSTM Architecture Diagram" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 2:</strong> Detailed water level forecasting LSTM architecture showing the multivariate input processing, temporal sequence modeling, and multi-step output generation for overflow prediction.</p>
      </div>
    </div>
  </div>
</div>

<div class="results-gallery">
  <h2><i class="fas fa-chart-bar text-primary"></i> Performance Analysis</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="performance-card">
        <h4><i class="fas fa-trophy"></i> Model Performance</h4>
        <ul class="metric-list">
          <li><strong>RMSE:</strong> 0.089 (normalized)</li>
          <li><strong>MAE:</strong> 0.067 (normalized)</li>
          <li><strong>Nash-Sutcliffe Efficiency:</strong> 0.94</li>
          <li><strong>RSR Ratio:</strong> 0.25</li>
        </ul>
      </div>
    </div>
    <div class="col-md-6">
      <div class="performance-card">
        <h4><i class="fas fa-exclamation-triangle"></i> Overflow Detection</h4>
        <ul class="metric-list">
          <li><strong>Overflow Prediction:</strong> 98.3% accuracy</li>
          <li><strong>Early Warning:</strong> 4-6 hour lead time</li>
          <li><strong>False Alarms:</strong> <5% rate</li>
          <li><strong>Critical Events:</strong> 100% detection</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="impact-section">
  <h2><i class="fas fa-medal text-warning"></i> Real-world Impact</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-shield-alt"></i> Operational Security</h4>
        <p>Provides water utilities with reliable early warning systems for overflow prevention, ensuring environmental protection and regulatory compliance.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-cogs"></i> Operational Efficiency</h4>
        <p>Enables proactive maintenance scheduling and resource allocation through accurate multi-step forecasting capabilities.</p>
      </div>
    </div>
  </div>
</div>
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
