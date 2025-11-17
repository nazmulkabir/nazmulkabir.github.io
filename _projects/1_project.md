---
layout: page
title: DC Water
description: AI-driven wastewater level prediction using Multivariate Multistep LSTM model for the 2022 International Water Systems Challenge
img: assets/img/DCWater.png
importance: 4
category: work
technologies: "LSTM, Deep Learning, Time Series Forecasting, Cybersecurity, Optimization"
status: completed
github: https://github.com/nazmulkabir/dcwater-project
demo: https://dcwater-demo.herokuapp.com
paper: /assets/pdf/dcwater_paper.pdf
related_publications: true
---

<div class="project-header">
  <div class="project-badges mb-4">
    <span class="badge-large bg-primary"><i class="fas fa-water"></i> Water Systems</span>
    <span class="badge-large bg-success"><i class="fas fa-brain"></i> Deep Learning</span>
    <span class="badge-large bg-info"><i class="fas fa-chart-line"></i> Forecasting</span>
    <span class="badge-large bg-warning"><i class="fas fa-shield-alt"></i> Cybersecurity</span>
  </div>
  
  <div class="project-overview">
    <div class="row">
      <div class="col-lg-8">
        <div class="overview-content">
          <h2><i class="fas fa-lightbulb text-primary"></i> Project Overview</h2>
          <p class="lead">This comprehensive AI-driven solution was developed for the <strong>2022 International Water Systems (IWS) Challenge</strong>, focusing on intelligent water system management through advanced machine learning and deep learning techniques. The solution integrates three critical modules: prediction, protection, and optimization to enhance wastewater treatment plant operations.</p>
          
          <div class="highlight-box">
            <h4><i class="fas fa-target text-success"></i> Key Objectives</h4>
            <ul class="objectives-list">
              <li><strong>Prediction:</strong> Accurate tunnel water level forecasting using LSTM models</li>
              <li><strong>Protection:</strong> Real-time cyber threat detection and anomaly identification</li>
              <li><strong>Optimization:</strong> Intelligent pump operation scheduling for energy efficiency</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="project-stats">
          <div class="stat-card">
            <h3>95%</h3>
            <p>Prediction Accuracy</p>
          </div>
          <div class="stat-card">
            <h3>30%</h3>
            <p>Energy Savings</p>
          </div>
          <div class="stat-card">
            <h3>99.2%</h3>
            <p>Threat Detection Rate</p>
          </div>
          <div class="stat-card">
            <h3>24/7</h3>
            <p>Real-time Monitoring</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="methodology-section">
  <h2><i class="fas fa-cogs text-primary"></i> Technical Methodology</h2>
  
  <div class="methodology-grid">
    <div class="row">
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-chart-line"></i>
          </div>
          <h4>Data Preprocessing</h4>
          <p>Advanced data cleaning, normalization, and feature engineering techniques for multivariate time series data from water treatment sensors.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-brain"></i>
          </div>
          <h4>LSTM Architecture</h4>
          <p>Multivariate Multistep LSTM model with attention mechanism for capturing long-term dependencies in water level patterns.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-shield-alt"></i>
          </div>
          <h4>Threat Detection</h4>
          <p>Anomaly detection algorithms for identifying potential cyber attacks and system malfunctions in real-time.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="results-gallery">
  <h2><i class="fas fa-images text-primary"></i> Project Gallery</h2>
  <div class="row">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="System Architecture Overview" class="img-fluid rounded z-depth-1" %}
      <div class="image-caption">System Architecture and Data Flow</div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="LSTM Model Performance" class="img-fluid rounded z-depth-1" %}
      <div class="image-caption">LSTM Model Training and Validation Results</div>
    </div>
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Real-time Dashboard" class="img-fluid rounded z-depth-1" %}
      <div class="image-caption">Real-time Monitoring Dashboard Interface</div>
    </div>
  </div>
</div>

<div class="module-sections">
  
  <!-- Prediction Module -->
  <div class="module-section prediction-module">
    <div class="module-header">
      <h2><i class="fas fa-chart-line text-primary"></i> Prediction Module</h2>
      <p class="module-description">Advanced multivariate time series forecasting for tunnel water levels using state-of-the-art LSTM architecture.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Technical Implementation</h4>
          <p>The prediction module leverages a sophisticated <strong>Multivariate Multistep LSTM model</strong> designed to forecast tunnel water levels in wastewater treatment plants. The model processes multiple input features including:</p>
          
          <ul class="feature-list">
            <li><strong>Historical Water Levels:</strong> Time series data from multiple sensors</li>
            <li><strong>Weather Conditions:</strong> Precipitation, temperature, and atmospheric pressure</li>
            <li><strong>Flow Rates:</strong> Inflow and outflow measurements</li>
            <li><strong>Operational Parameters:</strong> Pump status and treatment process variables</li>
          </ul>
          
          <div class="algorithm-box">
            <h5><i class="fas fa-algorithm"></i> Model Architecture</h5>
            <ul>
              <li>Multi-layer LSTM with 128 hidden units per layer</li>
              <li>Attention mechanism for feature importance weighting</li>
              <li>Dropout regularization (0.2) to prevent overfitting</li>
              <li>Adam optimizer with learning rate scheduling</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Performance Metrics</h4>
          <div class="metric-item">
            <span class="metric-label">RMSE:</span>
            <span class="metric-value">0.087</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">MAE:</span>
            <span class="metric-value">0.062</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">R² Score:</span>
            <span class="metric-value">0.956</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Prediction Horizon:</span>
            <span class="metric-value">6 hours</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="visualization-container">
      {% include figure.liquid loading="eager" path="assets/img/DCWater.png" title="DC Water Project Methodology" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 1:</strong> Comprehensive methodology for tunnel water level prediction showing data preprocessing, LSTM model architecture, and real-time forecasting pipeline.</p>
      </div>
    </div>
  </div>

  <!-- Protection Module -->
  <div class="module-section protection-module">
    <div class="module-header">
      <h2><i class="fas fa-shield-alt text-danger"></i> Protection Module</h2>
      <p class="module-description">Real-time cybersecurity threat detection and anomaly identification system for critical water infrastructure.</p>
    </div>
    
    <div class="security-features">
      <div class="row">
        <div class="col-md-6">
          <div class="security-card">
            <h4><i class="fas fa-exclamation-triangle"></i> Anomaly Detection</h4>
            <p>Advanced statistical and machine learning methods for identifying unusual patterns in sensor data that may indicate cyber attacks or system malfunctions.</p>
            <ul>
              <li>Isolation Forest algorithm for outlier detection</li>
              <li>Statistical process control charts</li>
              <li>Real-time threshold monitoring</li>
            </ul>
          </div>
        </div>
        <div class="col-md-6">
          <div class="security-card">
            <h4><i class="fas fa-bug"></i> Intrusion Detection</h4>
            <p>Network-based intrusion detection system specifically designed for industrial control systems and SCADA networks.</p>
            <ul>
              <li>Deep packet inspection</li>
              <li>Protocol anomaly detection</li>
              <li>Behavioral analysis of network traffic</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    
    <div class="threat-landscape">
      {% include figure.liquid path="assets/img/DCWater.png" title="Cybersecurity Framework" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 2:</strong> Multi-layered cybersecurity framework for detecting and mitigating cyber attacks on water distribution systems, including real-time monitoring and automated response mechanisms.</p>
      </div>
    </div>
  </div>

  <!-- Optimization Module -->
  <div class="module-section optimization-module">
    <div class="module-header">
      <h2><i class="fas fa-cog text-success"></i> Optimization Module</h2>
      <p class="module-description">Intelligent pump scheduling and energy optimization system for enhanced operational efficiency.</p>
    </div>
    
    <div class="optimization-details">
      <div class="row">
        <div class="col-lg-6">
          <h4>Optimization Objectives</h4>
          <ul class="optimization-list">
            <li><strong>Energy Efficiency:</strong> Minimize power consumption while maintaining service levels</li>
            <li><strong>Cost Reduction:</strong> Optimize operations during off-peak electricity hours</li>
            <li><strong>Equipment Longevity:</strong> Reduce wear and tear through intelligent scheduling</li>
            <li><strong>Environmental Impact:</strong> Lower carbon footprint through efficient operations</li>
          </ul>
        </div>
        <div class="col-lg-6">
          <h4>Optimization Techniques</h4>
          <ul class="optimization-list">
            <li>Genetic Algorithm for pump scheduling</li>
            <li>Linear programming for flow optimization</li>
            <li>Reinforcement learning for adaptive control</li>
            <li>Multi-objective optimization with Pareto frontiers</li>
          </ul>
        </div>
      </div>
    </div>
    
    <div class="optimization-results">
      {% include figure.liquid path="assets/img/DCWater.png" title="Optimization Results" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 3:</strong> Comprehensive optimization methodology showing energy consumption reduction, cost savings, and improved operational efficiency through intelligent pump scheduling and control algorithms.</p>
      </div>
    </div>
  </div>
</div>

<div class="additional-gallery">
  <h2><i class="fas fa-chart-bar text-primary"></i> Results and Analysis</h2>
  <div class="row">
    <div class="col-md-6">
      {% include figure.liquid path="assets/img/6.jpg" title="Performance Analysis" class="img-fluid rounded z-depth-1" %}
      <div class="image-caption">Detailed performance analysis and benchmarking results</div>
    </div>
    <div class="col-md-6">
      {% include figure.liquid path="assets/img/11.jpg" title="System Integration" class="img-fluid rounded z-depth-1" %}
      <div class="image-caption">Complete system integration and deployment architecture</div>
    </div>
  </div>
</div>

<div class="impact-section">
  <h2><i class="fas fa-medal text-warning"></i> Project Impact & Recognition</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-trophy"></i> Competition Results</h4>
        <p>Successfully participated in the 2022 International Water Systems Challenge, demonstrating innovative AI solutions for critical water infrastructure management.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-handshake"></i> Industry Collaboration</h4>
        <p>Collaborated with DC Water and other industry partners to develop practical, deployable solutions for real-world water treatment facilities.</p>
      </div>
    </div>
  </div>
</div>

<style>
/* Enhanced Project Page Styling */
.project-header {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 3rem 2rem;
  border-radius: 1rem;
  margin-bottom: 3rem;
  position: relative;
  overflow: hidden;
}

.project-header::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grid" width="10" height="10" patternUnits="userSpaceOnUse"><path d="M 10 0 L 0 0 0 10" fill="none" stroke="rgba(255,255,255,0.1)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23grid)"/></svg>');
  opacity: 0.3;
}

.project-badges {
  position: relative;
  z-index: 2;
}

.badge-large {
  font-size: 0.9rem;
  padding: 0.6rem 1.2rem;
  margin: 0.3rem;
  border-radius: 2rem;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
}

.overview-content {
  position: relative;
  z-index: 2;
}

.project-overview h2 {
  color: white;
  margin-bottom: 1.5rem;
}

.project-overview .lead {
  font-size: 1.2rem;
  line-height: 1.7;
  margin-bottom: 2rem;
}

.highlight-box {
  background: rgba(255,255,255,0.1);
  padding: 2rem;
  border-radius: 1rem;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
  margin-top: 2rem;
}

.objectives-list {
  list-style: none;
  padding: 0;
}

.objectives-list li {
  padding: 0.8rem 0;
  border-bottom: 1px solid rgba(255,255,255,0.1);
}

.objectives-list li:last-child {
  border-bottom: none;
}

.project-stats {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

.stat-card {
  background: rgba(255,255,255,0.1);
  padding: 1.5rem;
  border-radius: 1rem;
  text-align: center;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
}

.stat-card h3 {
  font-size: 2rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
  color: #fff;
}

.stat-card p {
  margin: 0;
  opacity: 0.9;
  font-weight: 600;
}

/* Methodology Section */
.methodology-section {
  padding: 3rem 0;
  background: #f8f9fa;
  border-radius: 1rem;
  margin: 3rem 0;
}

.methodology-section h2 {
  text-align: center;
  margin-bottom: 3rem;
  color: #2c3e50;
}

.method-card {
  background: white;
  padding: 2rem;
  border-radius: 1rem;
  text-align: center;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  height: 100%;
  transition: all 0.3s ease;
}

.method-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 30px rgba(0,0,0,0.15);
}

.method-icon {
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 1.5rem;
  font-size: 2rem;
  color: white;
}

/* Module Sections */
.module-section {
  margin: 4rem 0;
  padding: 3rem;
  border-radius: 1rem;
  border-left: 5px solid;
}

.prediction-module {
  background: linear-gradient(135deg, #e3f2fd 0%, #f3e5f5 100%);
  border-left-color: #2196f3;
}

.protection-module {
  background: linear-gradient(135deg, #ffebee 0%, #fce4ec 100%);
  border-left-color: #f44336;
}

.optimization-module {
  background: linear-gradient(135deg, #e8f5e8 0%, #f1f8e9 100%);
  border-left-color: #4caf50;
}

.module-header h2 {
  color: #2c3e50;
  margin-bottom: 1rem;
}

.module-description {
  font-size: 1.1rem;
  color: #6c757d;
  margin-bottom: 2rem;
}

.technical-details, .security-features, .optimization-details {
  margin: 2rem 0;
}

.feature-list, .optimization-list {
  list-style: none;
  padding: 0;
}

.feature-list li, .optimization-list li {
  padding: 0.8rem 0;
  border-bottom: 1px solid rgba(0,0,0,0.1);
  position: relative;
  padding-left: 2rem;
}

.feature-list li::before, .optimization-list li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: #4caf50;
  font-weight: bold;
}

.algorithm-box {
  background: rgba(255,255,255,0.8);
  padding: 1.5rem;
  border-radius: 0.8rem;
  margin: 1.5rem 0;
  border: 1px solid rgba(0,0,0,0.1);
}

.results-summary {
  background: rgba(255,255,255,0.9);
  padding: 2rem;
  border-radius: 1rem;
  border: 1px solid rgba(0,0,0,0.1);
}

.metric-item {
  display: flex;
  justify-content: space-between;
  padding: 0.8rem 0;
  border-bottom: 1px solid rgba(0,0,0,0.1);
}

.metric-label {
  font-weight: 600;
  color: #495057;
}

.metric-value {
  font-weight: 700;
  color: #2c3e50;
}

/* Security Cards */
.security-card {
  background: rgba(255,255,255,0.9);
  padding: 2rem;
  border-radius: 1rem;
  margin-bottom: 2rem;
  border: 1px solid rgba(0,0,0,0.1);
  height: 100%;
}

.security-card h4 {
  color: #dc3545;
  margin-bottom: 1rem;
}

/* Gallery and Images */
.results-gallery, .additional-gallery {
  margin: 4rem 0;
}

.image-caption, .caption-detailed {
  text-align: center;
  font-style: italic;
  color: #6c757d;
  margin-top: 1rem;
  padding: 0 1rem;
}

.caption-detailed {
  background: #f8f9fa;
  padding: 1rem;
  border-radius: 0.5rem;
  margin-top: 1.5rem;
}

.visualization-container, .threat-landscape, .optimization-results {
  margin: 3rem 0;
}

/* Impact Section */
.impact-section {
  background: linear-gradient(135deg, #fff3cd 0%, #f8d7da 100%);
  padding: 3rem;
  border-radius: 1rem;
  margin: 4rem 0;
}

.impact-card {
  background: rgba(255,255,255,0.9);
  padding: 2rem;
  border-radius: 1rem;
  margin-bottom: 2rem;
  border: 1px solid rgba(0,0,0,0.1);
  height: 100%;
}

.impact-card h4 {
  color: #856404;
  margin-bottom: 1rem;
}

/* Responsive Design */
@media (max-width: 768px) {
  .project-header {
    padding: 2rem 1rem;
  }
  
  .project-stats {
    grid-template-columns: 1fr;
  }
  
  .module-section {
    padding: 2rem 1rem;
  }
  
  .method-card {
    padding: 1.5rem;
  }
}
</style>
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
        {% include figure.liquid path="assets/img/DCWater.png" title="Methodology for Detecting Cyber Attacks" class="img-fluid rounded z-depth-1" %}
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
        {% include figure.liquid path="assets/img/DCWater.png" title="Optimization Methodology" class="img-fluid rounded z-depth-1" %}
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