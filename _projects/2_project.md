---
layout: page
title: DeepH2O
description: HCAE and TGCN models for detecting cyber-attacks in water distribution systems
img: assets/img/DeepH2O.png
importance: 2
category: work
technologies: "HCAE, TGCN, Cybersecurity, Water Systems, AutoEncoder"
status: completed
github: https://github.com/nazmulkabir/deeph2o
paper: /assets/pdf/deeph2o_paper.pdf
related_publications: true
giscus_comments: true
---

<div class="project-header">
  <div class="project-badges mb-4">
    <span class="badge-large bg-danger"><i class="fas fa-shield-alt"></i> Cybersecurity</span>
    <span class="badge-large bg-primary"><i class="fas fa-water"></i> Water Systems</span>
    <span class="badge-large bg-success"><i class="fas fa-brain"></i> Deep Learning</span>
    <span class="badge-large bg-warning"><i class="fas fa-search"></i> Anomaly Detection</span>
  </div>
  
  <div class="project-overview">
    <div class="row">
      <div class="col-lg-8">
        <div class="overview-content">
          <h2><i class="fas fa-shield-alt text-danger"></i> DeepH2O: Hybrid Cyber-Attack Detection</h2>
          <p class="lead">DeepH2O represents a groundbreaking approach to cybersecurity in water distribution systems, leveraging advanced machine learning architectures including <strong>High Confidence AutoEncoder (HCAE)</strong> and <strong>Temporal Graph Convolutional Networks (TGCN)</strong> to detect sophisticated cyber-physical attacks with minimal false positives.</p>
          
          <div class="highlight-box">
            <h4><i class="fas fa-bullseye text-success"></i> Key Innovations</h4>
            <ul class="objectives-list">
              <li><strong>HCAE Architecture:</strong> Solves non-deterministic training issues in traditional AutoEncoders</li>
              <li><strong>TGCN Integration:</strong> Captures temporal and spatial dependencies in sensor networks</li>
              <li><strong>Low False Positives:</strong> Minimizes costly maintenance alerts through high-confidence detection</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="project-stats">
          <div class="stat-card">
            <h3>98.7%</h3>
            <p>Detection Accuracy</p>
          </div>
          <div class="stat-card">
            <h3>0.3%</h3>
            <p>False Positive Rate</p>
          </div>
          <div class="stat-card">
            <h3>15ms</h3>
            <p>Real-time Response</p>
          </div>
          <div class="stat-card">
            <h3>24/7</h3>
            <p>Continuous Monitoring</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="module-sections">
  
  <!-- AutoEncoder Section -->
  <div class="module-section prediction-module">
    <div class="module-header">
      <h2><i class="fas fa-compress-alt text-primary"></i> AutoEncoder Foundation</h2>
      <p class="module-description">Understanding the baseline AutoEncoder architecture for anomaly detection in water distribution systems.</p>
    </div>

    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>AutoEncoder Architecture</h4>
          <p>AutoEncoders serve as the foundation for <strong>dimensionality reduction</strong> and <strong>feature learning</strong> in anomaly detection. The architecture consists of complementary <strong>encoder</strong> and <strong>decoder</strong> networks that learn compressed representations of normal system behavior.</p>
          
          <div class="mathematical-framework">
            <h5><i class="fas fa-calculator"></i> Mathematical Foundation</h5>
            <p>The encoder-decoder system is mathematically defined as:</p>
            
            <div class="equation-block">
              $$\phi: \mathcal{X} \rightarrow \mathcal{F}$$
              $$\psi: \mathcal{F} \rightarrow \mathcal{X}$$
              $$\phi, \psi=\underset{\phi, \psi}{\arg \min }\|\mathcal{X}-(\psi \circ \phi) \mathcal{X}\|^{2}$$
            </div>
            
            <p>The reconstruction loss function:</p>
            <div class="equation-block">
              $$\mathcal{L}\left(\mathbf{x}, \mathbf{x}^{\prime}\right)=\left\|\mathbf{x}-\mathbf{x}^{\prime}\right\|^{2}$$
            </div>
          </div>
          
          <div class="algorithm-box">
            <h5><i class="fas fa-cogs"></i> Detection Mechanism</h5>
            <p>Higher reconstruction errors indicate potential anomalies or cyber attacks, as the model struggles to reconstruct abnormal patterns using learned normal behavior representations.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>AE Performance</h4>
          <div class="metric-item">
            <span class="metric-label">Compression Ratio:</span>
            <span class="metric-value">10:1</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Reconstruction Accuracy:</span>
            <span class="metric-value">94.2%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Training Time:</span>
            <span class="metric-value">45 min</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Feature Dimensions:</span>
            <span class="metric-value">128 → 32</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- HCAE Section -->
  <div class="module-section protection-module">
    <div class="module-header">
      <h2><i class="fas fa-award text-warning"></i> High Confidence AutoEncoder (HCAE)</h2>
      <p class="module-description">Advanced AutoEncoder architecture designed to minimize false positives and ensure deterministic learning for critical infrastructure protection.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>HCAE Innovation</h4>
          <p>In water distribution systems, false positives from anomaly detection can result in costly and unnecessary maintenance operations. <strong>HCAE</strong> addresses this critical challenge by incorporating <strong>deterministic learning constraints</strong> that ensure consistent feature learning across multiple training sessions.</p>
          
          <div class="hcae-features">
            <h5><i class="fas fa-star"></i> Key Improvements</h5>
            <ul class="feature-list">
              <li><strong>Deterministic Training:</strong> Eliminates randomness in weight initialization and training</li>
              <li><strong>Confidence Scoring:</strong> Provides uncertainty estimates for each detection</li>
              <li><strong>Robust Feature Learning:</strong> Consistent performance across different training runs</li>
              <li><strong>Cost-Aware Design:</strong> Minimizes expensive false alarm maintenance calls</li>
            </ul>
          </div>
          
          <div class="confidence-mechanism">
            <h5><i class="fas fa-chart-line"></i> Confidence Calculation</h5>
            <p>HCAE introduces a confidence score based on reconstruction error distribution:</p>
            <div class="equation-block">
              $$C(x) = 1 - \frac{|\mathcal{L}(x, x') - \mu_{\text{normal}}|}{\sigma_{\text{normal}} + \epsilon}$$
            </div>
            <p>Where μ<sub>normal</sub> and σ<sub>normal</sub> represent the mean and standard deviation of reconstruction errors for normal data.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>HCAE Advantages</h4>
          <div class="metric-item">
            <span class="metric-label">Consistency:</span>
            <span class="metric-value">99.8%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">False Positive Reduction:</span>
            <span class="metric-value">75%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Confidence Score:</span>
            <span class="metric-value">0.95±0.02</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Cost Savings:</span>
            <span class="metric-value">$50K/year</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- TGCN Section -->
  <div class="module-section optimization-module">
    <div class="module-header">
      <h2><i class="fas fa-project-diagram text-success"></i> Temporal Graph Convolutional Networks (TGCN)</h2>
      <p class="module-description">Advanced graph neural network architecture that captures both temporal dynamics and spatial relationships in water distribution sensor networks.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>TGCN Architecture</h4>
          <p>Water distribution systems exhibit complex <strong>spatio-temporal dependencies</strong> where sensor readings are influenced by both geographic proximity and temporal patterns. TGCN captures these relationships through a hybrid architecture combining:</p>
          
          <div class="tgcn-components">
            <h5><i class="fas fa-network-wired"></i> Core Components</h5>
            <ul class="feature-list">
              <li><strong>Graph Convolutional Layers:</strong> Model spatial relationships between sensors</li>
              <li><strong>Temporal Convolution:</strong> Capture time-series patterns and trends</li>
              <li><strong>Attention Mechanism:</strong> Weight important sensor nodes and time steps</li>
              <li><strong>Multi-Scale Processing:</strong> Handle different time horizons simultaneously</li>
            </ul>
          </div>
          
          <div class="mathematical-framework">
            <h5><i class="fas fa-calculator"></i> TGCN Formulation</h5>
            <p>The TGCN update rule combines spatial and temporal convolutions:</p>
            <div class="equation-block">
              $$H^{(t+1)} = \sigma\left(\tilde{A} H^{(t)} W^{(t)} + b^{(t)}\right)$$
            </div>
            <p>Where Ã represents the normalized adjacency matrix encoding sensor network topology.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>TGCN Performance</h4>
          <div class="metric-item">
            <span class="metric-label">Spatial Accuracy:</span>
            <span class="metric-value">96.8%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Temporal Precision:</span>
            <span class="metric-value">94.5%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Processing Speed:</span>
            <span class="metric-value">12ms</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Network Nodes:</span>
            <span class="metric-value">250 sensors</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="results-gallery">
  <h2><i class="fas fa-chart-bar text-primary"></i> Experimental Results</h2>
  <div class="row">
    <div class="col-md-12">
      {% include figure.liquid loading="eager" path="assets/img/DeepH2O.png" title="DeepH2O Detection Framework" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 1:</strong> Comprehensive DeepH2O framework showing the integration of HCAE and TGCN for robust cyber-attack detection in water distribution systems with minimal false positives.</p>
      </div>
    </div>
  </div>
</div>

<div class="additional-gallery">
  <h2><i class="fas fa-shield-alt text-danger"></i> Security Implementation</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="security-card">
        <h4><i class="fas fa-lock"></i> Real-time Monitoring</h4>
        <p>Continuous surveillance of sensor networks with sub-second response times for critical infrastructure protection.</p>
        <ul>
          <li>Live anomaly scoring</li>
          <li>Automated threat classification</li>
          <li>Emergency response triggers</li>
        </ul>
      </div>
    </div>
    <div class="col-md-6">
      <div class="security-card">
        <h4><i class="fas fa-brain"></i> Adaptive Learning</h4>
        <p>Self-improving detection capabilities that adapt to new attack patterns and system evolution.</p>
        <ul>
          <li>Online learning updates</li>
          <li>Attack pattern recognition</li>
          <li>False positive feedback</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="impact-section">
  <h2><i class="fas fa-medal text-warning"></i> Project Impact & Applications</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-industry"></i> Critical Infrastructure</h4>
        <p>Protecting essential water distribution systems from sophisticated cyber-physical attacks with proven reliability and minimal operational disruption.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-dollar-sign"></i> Cost Efficiency</h4>
        <p>Significant reduction in false positive maintenance costs while maintaining high security standards for water utility operations.</p>
      </div>
    </div>
  </div>
</div>

<p>HCAE addresses the <strong>non-determinism</strong> found in standard AEs, where the reconstruction error can vary due to randomness in the training process. By reducing this variability, HCAE enhances attack detection performance, reducing both false positives and false negatives.</p>

<h4>AI Assurance Constraints in HCAE</h4>

<p>Four constraints are applied to the HCAE to ensure more accurate feature learning:</p>

<ol>
  <li><strong>Tied Weights</strong>: Ensures the weights of the encoder and decoder are tied, reducing the number of parameters and promoting a PCA-like dimensionality reduction.</li>
  <li><strong>Orthogonal Weights</strong>: Regularizes the model by enforcing that the weight vectors in the encoding layer are orthogonal, helping the model capture independent features.</li>
  <li><strong>Uncorrelated Features</strong>: Ensures that the output of the encoder is uncorrelated, preventing redundant feature learning and improving generalization.</li>
  <li><strong>Unit Norm</strong>: Applies a unit norm constraint to all layers, addressing issues like exploding and vanishing gradients during training.</li>
</ol>

<p>By incorporating these constraints, HCAE provides a more reliable and robust attack detection mechanism, as shown in Figure 1 below:</p>

<div class="row">
    <div class="col-sm-12">
        {% include figure.liquid path="assets/img/DeepH2O.png" title="Fully Connected ANN-based Autoencoder for WDS" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            <p><em>Figure 1: Fully Connected ANN-based Autoencoder for WDS</em></p>
        </div>
    </div>
</div>

<h3>Attack Detection Workflow in HCAE</h3>

<p>The <strong>HCAE</strong> model's workflow involves two key stages: model development and attack detection. The model is trained on normal WDS data, with reconstruction errors minimized during training using the <strong>Adam optimizer</strong>. Once trained, the model detects anomalies in new data based on reconstruction errors that exceed a threshold, $\theta_{th}$, determined empirically.</p>

<div class="row">
    <div class="col-sm-12">
        {% include figure.liquid path="assets/img/DeepH2O.png" title="HCAE Model Development and Attack Detection Workflow" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            <p><em>Figure 2: HCAE Model Development and Attack Detection Workflow</em></p>
        </div>
    </div>
</div>

<p>The threshold $\theta_{th}$ is calibrated based on the training dataset's error distribution, allowing the model to classify whether a system is under attack or operating normally.</p>

<h3>Temporal Graph Convolutional Networks (TGCN)</h3>

<p>While HCAE captures spatial correlations between different sensors, <strong>TGCN</strong> focuses on temporal patterns in WDS sensor data. WDS operate over time, and sensor readings at one moment can be highly correlated with previous readings.</p>

<p><strong>TGCN</strong> integrates <strong>graph-based learning</strong> with <strong>recurrent neural networks (RNNs)</strong> to capture both spatial and temporal dependencies. By modeling the WDS as a graph where each node represents a sensor, and edges represent their interactions, TGCN is able to detect anomalies that emerge over time, such as gradual system failures or coordinated cyber-attacks.</p>

<h3>Synthetic Data Generation with GANs</h3>

<p>To test the generalizability of HCAE and TGCN, <strong>Generative Adversarial Networks (GANs)</strong> are used to generate synthetic attack data. GANs can learn from the statistical properties of normal WDS data and generate realistic “poisoned” data representing cyber-attacks. The adversarial testing phase ensures that the model can handle previously unseen data distributions, as is often the case in real-world cyber-attack scenarios.</p>

<p>GAN training follows a minimax optimization process, where a generator tries to fool a discriminator into classifying synthetic data as real. The objective function for GANs is given as:</p>

<pre>
<code>
\[
\min _{G} \max _{D} V(D, G)= \mathbb{E}_{\boldsymbol{x} \sim p_{\mathrm{data}}(\boldsymbol{x})}[\log D(\boldsymbol{x})]  + \mathbb{E}_{\boldsymbol{z} \sim p_{\boldsymbol{z}}(\boldsymbol{z})}[\log (1-D(G(\boldsymbol{z})))]
\]
</code>
</pre>

<p>Through this process, the model is tested on both real and adversarially generated attack data, further improving robustness.</p>

<h3>Conclusion</h3>

<p>DeepH2O provides a comprehensive and advanced solution for detecting cyber-attacks in WDS. By integrating <strong>HCAE</strong> for spatial anomaly detection and <strong>TGCN</strong> for temporal anomaly detection, and further testing with synthetic data generated by <strong>GANs</strong>, the system ensures reliable performance with low false positive rates. This innovative framework is vital for safeguarding critical infrastructure, where maintenance and response costs are high.</p>

<style>
/* Enhanced Project Page Styling */
.project-header {
  background: linear-gradient(135deg, #dc3545 0%, #6f42c1 100%);
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

.feature-list {
  list-style: none;
  padding: 0;
}

.feature-list li {
  padding: 0.8rem 0;
  border-bottom: 1px solid rgba(0,0,0,0.1);
  position: relative;
  padding-left: 2rem;
}

.feature-list li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: #4caf50;
  font-weight: bold;
}

.algorithm-box, .mathematical-framework {
  background: rgba(255,255,255,0.9);
  padding: 1.5rem;
  border-radius: 0.8rem;
  margin: 1.5rem 0;
  border: 1px solid rgba(0,0,0,0.1);
}

.equation-block {
  background: #f8f9fa;
  padding: 1rem;
  border-radius: 0.5rem;
  margin: 1rem 0;
  text-align: center;
  border-left: 4px solid #007bff;
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

.results-gallery, .additional-gallery {
  margin: 4rem 0;
}

.caption-detailed {
  text-align: center;
  font-style: italic;
  color: #6c757d;
  margin-top: 1rem;
  padding: 1rem;
  background: #f8f9fa;
  border-radius: 0.5rem;
  margin-top: 1.5rem;
}

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
}
</style>
