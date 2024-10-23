---
layout: page
title: WcdNet-RNN
description: Context aware Deep Learning based solution for water systems
img: assets/img/context.png
importance: 1
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/context.png" title="WcdNet-RNN Model Overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Overview of WcdNet-RNN for short-term water level forecasting in water system services (WSS).
</div>

### Problem Statement: Short-Term Water Level Forecasting (STWLF)

The objective of short-term water level forecasting is to predict inflow levels over a short horizon. Specifically, we aim to forecast future water levels \( \{y_t\}_{M+1}^{M+H} \) based on past data \( \{y_t\}_{1}^{M} \), where:

\[
y_t = \text{Water level at time } t
\]
\[
M = \text{Length of historical data}
\]
\[
H = \text{Forecast horizon (e.g., 4-6 hours)}
\]

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flow_diagram.png" title="Flow Diagram of WcdNet-RNN Stages" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The flow diagram illustrates the two main stages of WcdNet-RNN: context extraction and forecasting.
</div>

### WcdNet-RNN Architecture

Each time series is decomposed into its seasonal component \( S_t \) and level component \( L_t \), with the dynamic smoothing method using the Holt-Winters model. The key smoothing equations are as follows:

\[
L_t = \alpha_t Y_t + (1 - \alpha_t)L_{t-1}
\]
\[
S_{t+P} = \beta_t \frac{Y_t}{L_t} + (1 - \beta_t)S_t
\]

Where \( L_t \) represents the level component, \( S_t \) represents the seasonal component, and \( \alpha_t, \beta_t \) are smoothing coefficients dynamically adjusted by the RNN.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/RNN_structure.png" title="RNN Structure for Forecasting" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Structure of the recurrent neural network (RNN) used in WcdNet-RNN for water inflow prediction.
</div>

### Loss Function

To optimize forecasts, WcdNet-RNN uses a pinball loss function for both point forecasts and predictive intervals. The loss function is defined as:

\[
L_{\tau} = \rho(y_{\tau}, \hat{y}_{q*, \tau}) + \gamma(\rho(y_{\tau}, \hat{y}_{q, \tau}) + \rho(y_{\tau}, \hat{y}_{\bar{q}, \tau}))
\]

Where \( \rho \) represents the pinball loss, \( q^* \) is the median quantile, and \( q, \bar{q} \) represent the bounds of the predictive intervals.

### Pre and Post-Processing

Preprocessing includes normalization and deseasonalization, while postprocessing applies inverse normalization and reintroduces patterns removed earlier. This ensures that forecasts are accurate and well-adjusted to changes in seasonal components.

### Conclusion

The WcdNet-RNN model provides a robust framework for short-term water level forecasting in water systems. By incorporating external context data such as weather and river levels, the model improves forecast accuracy.

