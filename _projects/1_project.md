---
layout: page
title: DC Water
description: Waste water level prediction using Multivariate Multistep LSTM model
img: assets/img/DCWater.png
importance: 4
category: work
related_publications: true
---

<p>This page provides an overview of the AI-driven solution developed for the 2022 International Water Systems (IWS) Challenge. The solution focuses on water system management through prediction, protection, and optimization modules using machine learning (ML) and deep learning (DL) techniques. These modules aid in managing wastewater levels, detecting cyber threats, and optimizing pump operations in water treatment plants (WWTPs).</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<h3>Prediction Module</h3>
<p>This module focuses on predicting tunnel water levels in WWTPs using ML and DL models. Figure 1 below illustrates the methodology used for tunnel water level prediction.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/Figure_3.pdf" alt="Methodology for Tunnel Water Level Prediction" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 1: Methodology for Tunnel Water Level Prediction.</em></p>
        </div>
    </div>
</div>

<p>The prediction module consists of five steps: Data Preprocessing, Exploratory Data Analysis (EDA), Model Development, Hyperparameter Tuning, and Model Evaluation. After data preprocessing, two versions of the data are created based on Principal Component Analysis (PCA) and downsampling methods to improve model assurance.</p>

<h4>Data Preprocessing for Wastewater-level Prediction</h4>
<p>The data used in this study contains 243 columns, with sensor readings requiring thorough preprocessing. This step involves handling missing (NA) values, selecting relevant features, and creating multiple versions of the dataset for model development.</p>

<h4>Model Selection and Development</h4>
<p>Several ML models, including Random Forest (RF), eXtreme Gradient Boosting (XGBoost), and LightGBM, were selected alongside two DL models: Feed Forward Artificial Neural Network (FF-ANN) and Long Short-Term Memory (LSTM). These models were chosen based on their performance for multivariate time-series forecasting.</p>

<h4>Hyperparameter Tuning and Model Evaluation</h4>
<p>Hyperparameter tuning was conducted using grid search for tree-based models and random search for DL models. Evaluation metrics, such as Root Mean Squared Error (RMSE), Nash-Sutcliffe Efficiency (NSE), and RMSE-observation standard deviation ratio (RSR), were used to compare the models.</p>

<h3>Protection Module</h3>
<p>This module focuses on detecting and classifying cyber-physical attacks in WWTPs. The methodology uses the SMOD dataset, which includes sensor data from Programmable Logic Controllers (PLCs) to classify potential attack scenarios.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/Figure_4.pdf" alt="Methodology for Detecting Cyber Attacks" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 2: Methodology for Detecting Cyber Attacks.</em></p>
        </div>
    </div>
</div>

<p>Data preprocessing, model development, and evaluation techniques are discussed. The dataset was oversampled using the SMOTE technique to address imbalanced class distributions. LSTM and GRU models were developed and compared for accuracy, precision, recall, and F1-score metrics to identify and classify attack intentions.</p>

<h4>Results of Protection Module</h4>
<p>Overall, the LSTM model showed higher accuracy for classifying attacks, achieving over 95% accuracy in detecting intentional attacks. The GRU model, however, performed better in terms of misclassification rate for outlier events.</p>

<h3>Optimization Module</h3>
<p>This module optimizes pump operations in WWTPs to reduce the amount of wastewater directed to the wet-weather treatment plant (WWTP) during extreme weather events. The optimization problem is solved using a Genetic Algorithm (GA), which determines the optimal pump operation schedule to prevent overflow incidents.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/Figure_5.pdf" alt="Optimization Methodology" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 3: Optimization Methodology for Pump Operations.</em></p>
        </div>
    </div>
</div>

<p>The GA model was tested with a variety of scenarios and reduced the influent to the wet-weather treatment plant by 23%, preventing overflow incidents over five years of test data. The optimization is based on real-time predictions from the LSTM model.</p>

<h3>Results</h3>
<p>The results from all three modules (Prediction, Protection, and Optimization) demonstrate the efficacy of the AI-driven solution for managing WWTPs during extreme weather conditions. The LSTM model provided the most accurate predictions for wastewater levels, and the optimization module successfully recommended actionable steps to avoid overflow scenarios. Additionally, the protection module effectively detected and classified cyber-physical attacks, improving the overall security of the system.</p>

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<h3>Conclusion</h3>
<p>The 2022 IWS Challenge AI solution for water systems provides an integrated approach to wastewater management. Combining prediction, protection, and optimization modules helps in making informed decisions, ensuring operational efficiency, and safeguarding water treatment plants against potential threats. The graphical user interface of P<sub>2</sub>O offers real-time insights for plant operators, helping them manage both day-to-day operations and emergency situations efficiently.</p>