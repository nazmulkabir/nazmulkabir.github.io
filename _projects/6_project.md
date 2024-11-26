---
layout: page
title: cP2O
description: Context aware Deep Learning solution for water systems
img: assets/img/context.png
importance: 1
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/context_1.png" title="cP2O Model Overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Overview of cP2O for short-term water level forecasting in water system services (WSS).
</div>

### Problem Statement: Short-Term Water Level Forecasting (STWLF)

The objective of short-term water level forecasting is to predict inflow levels over a short horizon. Specifically, we aim to forecast future water levels $$ \{y_t\}_{M+1}^{M+H} $$ based on past data $$ \{y_t\}_{1}^{M} $$, where:

\begin{equation}
y_t = \text{Water level at time } t
\end{equation}
\begin{equation}
M = \text{Length of historical data}
\end{equation}
\begin{equation}
H = \text{Forecast horizon (e.g., 4-6 hours)}
\end{equation}

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/context_2.png" title="Dilated LSTM with Attention Mechanism and Hiarchical Dilated RNN Layers"  class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The flow diagram illustrates the two main stages of cP2O: context extraction and forecasting.
</div>

### cP2O Architecture

Each time series is decomposed into its seasonal component \( S_t \) and level component \( L_t \), with the dynamic smoothing method using the Holt-Winters model. The key smoothing equations are as follows:

\begin{equation}
L_t = \alpha_t Y_t + (1 - \alpha_t)L_{t-1}
\end{equation}
\begin{equation}
S_{t+P} = \beta_t \frac{Y_t}{L_t} + (1 - \beta_t)S_t
\end{equation}

Where \( L_t \) represents the level component, \( S_t \) represents the seasonal component, and \( \alpha_t, \beta_t \) are smoothing coefficients dynamically adjusted by the RNN.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/context_3.png" title="The cP2Oe forecasting results on WWTP data are presented, with actual values shown in blue, forecasts in red, and predictive intervals depicted in light gray shades" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Structure of the recurrent neural network (RNN) used in cP2O for water inflow prediction.
</div>

### Loss Function

To optimize forecasts, cP2O uses a pinball loss function for both point forecasts and predictive intervals. The loss function is defined as:

\begin{equation}
L_{\tau} = \rho(y_{\tau}, \hat{y}_{q^* , \tau}) + \gamma \left( \rho(y_{\tau}, \hat{y}_{q , \tau}) + \rho(y_{\tau}, \hat{y}_{\bar{q}, \tau}) \right)
\end{equation}

Where \\( \rho \\) represents the pinball loss, \\( q^* \\) is the median quantile, and \\( q, \bar{q} \\) represent the bounds of the predictive intervals.


### Pre and Post-Processing

Preprocessing includes normalization and deseasonalization, while postprocessing applies inverse normalization and reintroduces patterns removed earlier. This ensures that forecasts are accurate and well-adjusted to changes in seasonal components.

### Conclusion

The cP2O model provides a robust framework for short-term water level forecasting in water systems. By incorporating external context data such as weather and river levels, the model improves forecast accuracy.

