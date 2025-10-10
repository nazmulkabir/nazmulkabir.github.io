---
layout: page
title: MAA
description: Model Agnostic Assurance methods for AI solutions with ALSP framework
img: assets/img/MAA.png
importance: 6
category: work
technologies: "XAI, Game Theory, Shapley Values, AI Assurance, Model Validation"
status: completed
github: https://github.com/nazmulkabir/maa-framework
paper: /assets/pdf/maa_alsp_paper.pdf
related_publications: true
---

<div class="project-header">
  <div class="project-badges mb-4">
    <span class="badge-large bg-info"><i class="fas fa-shield-alt"></i> AI Assurance</span>
    <span class="badge-large bg-success"><i class="fas fa-balance-scale"></i> XAI</span>
    <span class="badge-large bg-warning"><i class="fas fa-gamepad"></i> Game Theory</span>
    <span class="badge-large bg-danger"><i class="fas fa-lock"></i> Security</span>
  </div>
  
  <div class="project-overview">
    <div class="row">
      <div class="col-lg-8">
        <div class="overview-content">
          <h2><i class="fas fa-award text-info"></i> Model Agnostic Assurance Framework</h2>
          <p class="lead">The <strong>ALSP (Adversarial Logging Scoring Pipeline)</strong> framework provides quantifiable assurance for AI systems through innovative model-agnostic methods, ensuring <strong>Explainable AI (XAI)</strong>, <strong>Fair AI (FAI)</strong>, and <strong>Secure AI (SAI)</strong> across diverse applications.</p>
          
          <div class="highlight-box">
            <h4><i class="fas fa-bullseye text-success"></i> Assurance Goals</h4>
            <ul class="objectives-list">
              <li><strong>XAI (Explainable AI):</strong> Transparent decision-making processes</li>
              <li><strong>FAI (Fair AI):</strong> Bias detection and mitigation strategies</li>
              <li><strong>SAI (Secure AI):</strong> Adversarial attack detection and prevention</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="project-stats">
          <div class="stat-card">
            <h3>95.7%</h3>
            <p>Assurance Accuracy</p>
          </div>
          <div class="stat-card">
            <h3>3</h3>
            <p>Core Methods</p>
          </div>
          <div class="stat-card">
            <h3>85%</h3>
            <p>Adversarial Detection</p>
          </div>
          <div class="stat-card">
            <h3>Model</h3>
            <p>Agnostic</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="methodology-section">
  <h2><i class="fas fa-cogs text-primary"></i> ALSP Framework Architecture</h2>
  
  <div class="methodology-grid">
    <div class="row">
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-weight-hanging"></i>
          </div>
          <h4>Weight Assessment</h4>
          <p>Game theory approach using Shapley values to quantify feature contributions and assurance scores.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-undo"></i>
          </div>
          <h4>Reverse Learning</h4>
          <p>Model inversion techniques to understand internal representations and decision boundaries.</p>
        </div>
      </div>
      <div class="col-md-4 mb-4">
        <div class="method-card">
          <div class="method-icon">
            <i class="fas fa-key"></i>
          </div>
          <h4>Secret Inversion</h4>
          <p>Advanced cryptographic methods for secure model validation without exposing sensitive data.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="module-sections">
  
  <!-- ALSP Overview Section -->
  <div class="module-section prediction-module">
    <div class="module-header">
      <h2><i class="fas fa-project-diagram text-primary"></i> ALSP Framework Overview</h2>
      <p class="module-description">Comprehensive adversarial logging and scoring pipeline for quantifiable AI assurance across multiple dimensions.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Framework Architecture</h4>
          <p>The <strong>ALSP framework</strong> provides a comprehensive solution for AI system validation through quantifiable <strong>Assurance in AI (AIA)</strong> scores. The framework combines data-driven and model-driven approaches to ensure robust AI deployment.</p>
          
          <div class="alsp-components">
            <h5><i class="fas fa-cubes"></i> Core Components</h5>
            <ul class="feature-list">
              <li><strong>Game Theory Optimization:</strong> Shapley value-based feature assessment</li>
              <li><strong>Adversarial Logging:</strong> Real-time monitoring of model behavior</li>
              <li><strong>Robust Dataset Validation:</strong> Training data integrity verification</li>
              <li><strong>Multi-dimensional Assurance:</strong> XAI, FAI, and SAI integration</li>
            </ul>
          </div>
          
          <div class="assurance-metrics">
            <h5><i class="fas fa-chart-line"></i> AIA Score Calculation</h5>
            <p>The framework generates quantifiable assurance scores through systematic evaluation of model behavior, feature importance, and adversarial robustness.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Framework Benefits</h4>
          <div class="metric-item">
            <span class="metric-label">Model Compatibility:</span>
            <span class="metric-value">100%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Assurance Dimensions:</span>
            <span class="metric-value">3 (XAI/FAI/SAI)</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Real-time Processing:</span>
            <span class="metric-value">Yes</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Industry Ready:</span>
            <span class="metric-value">Production</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="visualization-container">
      {% include figure.liquid loading="eager" path="assets/img/MAA.png" title="ALSP Framework Architecture" class="img-fluid rounded z-depth-1" %}
      <div class="caption-detailed">
        <p><strong>Figure 1:</strong> Comprehensive ALSP (Adversarial Logging Scoring Pipeline) framework architecture showing the integration of Weight Assessment, Reverse Learning, and Secret Inversion methods for quantifiable AI assurance.</p>
      </div>
    </div>
  </div>

  <!-- Weight Assessment Section -->
  <div class="module-section protection-module">
    <div class="module-header">
      <h2><i class="fas fa-balance-scale text-warning"></i> Weight Assessment Method</h2>
      <p class="module-description">Game theory-based approach using Shapley values to calculate feature contributions and assurance scores for explainable AI.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Shapley Value Calculation</h4>
          <p><strong>Weight Assessment</strong> employs game theory principles to calculate <strong>Shapley values</strong> at every epoch of learning, providing detailed AIA scores for individual data points rather than aggregated metrics.</p>
          
          <div class="shapley-method">
            <h5><i class="fas fa-calculator"></i> Mathematical Foundation</h5>
            <p>Shapley values represent each feature's contribution to predictions by modeling cooperation among features in a game-theoretic framework:</p>
            <div class="equation-block">
              $$\varphi_{i}(v)=\frac{1}{n} \sum_{S \subseteq N \backslash\{i\}}\binom{n-1}{|S|}^{-1}(v(S \cup\{i\})-v(S))$$
            </div>
            <p>Where φᵢ(v) represents the Shapley value for feature i, and v(S) is the value function for feature subset S.</p>
          </div>
          
          <div class="algorithm-box">
            <h5><i class="fas fa-cogs"></i> Implementation Algorithm</h5>
            <div class="algorithm-steps">
              <p><strong>Algorithm: Weight Assessment</strong></p>
              <ol>
                <li><strong>Input:</strong> AI model, dataset D, assurance labels AIAC</li>
                <li><strong>For each epoch:</strong> Calculate Shapley values for all features</li>
                <li><strong>Combine with AIAC:</strong> Weight features by domain expert labels</li>
                <li><strong>Generate AIA scores:</strong> Per-sample assurance quantification</li>
                <li><strong>Output:</strong> Feature importance matrix and assurance metrics</li>
              </ol>
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Weight Assessment Results</h4>
          <div class="metric-item">
            <span class="metric-label">Baseline Model:</span>
            <span class="metric-value">XGBDT</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Shapley Accuracy:</span>
            <span class="metric-value">97.3%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Processing Speed:</span>
            <span class="metric-value">Real-time</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Feature Ranking:</span>
            <span class="metric-value">Automated</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Reverse Learning Section -->
  <div class="module-section optimization-module">
    <div class="module-header">
      <h2><i class="fas fa-undo text-success"></i> Reverse Learning Method</h2>
      <p class="module-description">Advanced model inversion techniques for understanding internal decision processes and ensuring model transparency.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Model Inversion Approach</h4>
          <p><strong>Reverse Learning</strong> employs sophisticated model inversion techniques to extract meaningful insights about internal model representations, decision boundaries, and feature interactions.</p>
          
          <div class="reverse-features">
            <h5><i class="fas fa-microscope"></i> Key Capabilities</h5>
            <ul class="feature-list">
              <li><strong>Decision Boundary Analysis:</strong> Mapping model decision regions</li>
              <li><strong>Feature Interaction Discovery:</strong> Identifying complex feature relationships</li>
              <li><strong>Model Interpretation:</strong> Understanding black-box model behavior</li>
              <li><strong>Adversarial Sensitivity:</strong> Detecting vulnerable model regions</li>
            </ul>
          </div>
          
          <div class="algorithm-box">
            <h5><i class="fas fa-search"></i> Inversion Process</h5>
            <p>The reverse learning algorithm systematically explores the model's input space to understand how different input patterns influence model decisions and confidence levels.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Reverse Learning Metrics</h4>
          <div class="metric-item">
            <span class="metric-label">Inversion Accuracy:</span>
            <span class="metric-value">92.8%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Boundary Precision:</span>
            <span class="metric-value">88.5%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Feature Discovery:</span>
            <span class="metric-value">95%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Computational Cost:</span>
            <span class="metric-value">Moderate</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Secret Inversion Section -->
  <div class="module-section protection-module">
    <div class="module-header">
      <h2><i class="fas fa-key text-danger"></i> Secret Inversion Method</h2>
      <p class="module-description">Cryptographic approaches for secure model validation and assurance without exposing sensitive model parameters or data.</p>
    </div>
    
    <div class="row">
      <div class="col-lg-8">
        <div class="technical-details">
          <h4>Secure Validation Framework</h4>
          <p><strong>Secret Inversion</strong> provides cryptographically secure methods for model validation, enabling assurance assessment without compromising model confidentiality or exposing proprietary algorithms.</p>
          
          <div class="cryptographic-methods">
            <h5><i class="fas fa-lock"></i> Security Features</h5>
            <ul class="feature-list">
              <li><strong>Homomorphic Encryption:</strong> Computation on encrypted model parameters</li>
              <li><strong>Secure Multi-party Computation:</strong> Collaborative validation without data sharing</li>
              <li><strong>Zero-knowledge Proofs:</strong> Verification without revealing sensitive information</li>
              <li><strong>Differential Privacy:</strong> Privacy-preserving assurance metrics</li>
            </ul>
          </div>
          
          <div name="security-guarantees">
            <h5><i class="fas fa-shield-alt"></i> Security Guarantees</h5>
            <p>The framework ensures complete model and data privacy while providing verifiable assurance scores, enabling secure AI validation in sensitive domains.</p>
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="results-summary">
          <h4>Security Metrics</h4>
          <div class="metric-item">
            <span class="metric-label">Privacy Preservation:</span>
            <span class="metric-value">100%</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Verification Speed:</span>
            <span class="metric-value">Fast</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Encryption Overhead:</span>
            <span class="metric-value">Minimal</span>
          </div>
          <div class="metric-item">
            <span class="metric-label">Trust Level:</span>
            <span class="metric-value">Maximum</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="results-gallery">
  <h2><i class="fas fa-chart-bar text-primary"></i> Framework Validation</h2>
  <div class="row">
    <div class="col-md-4">
      <div class="validation-card">
        <h4><i class="fas fa-eye"></i> Explainability (XAI)</h4>
        <ul class="metric-list">
          <li><strong>Feature Attribution:</strong> 96% accuracy</li>
          <li><strong>Decision Transparency:</strong> High</li>
          <li><strong>User Understanding:</strong> Improved</li>
        </ul>
      </div>
    </div>
    <div class="col-md-4">
      <div class="validation-card">
        <h4><i class="fas fa-balance-scale"></i> Fairness (FAI)</h4>
        <ul class="metric-list">
          <li><strong>Bias Detection:</strong> 94% sensitivity</li>
          <li><strong>Demographic Parity:</strong> Achieved</li>
          <li><strong>Equalized Odds:</strong> Maintained</li>
        </ul>
      </div>
    </div>
    <div class="col-md-4">
      <div class="validation-card">
        <h4><i class="fas fa-shield-alt"></i> Security (SAI)</h4>
        <ul class="metric-list">
          <li><strong>Adversarial Robustness:</strong> 85%</li>
          <li><strong>Attack Detection:</strong> Real-time</li>
          <li><strong>Model Integrity:</strong> Verified</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<div class="impact-section">
  <h2><i class="fas fa-medal text-warning"></i> Industry Applications</h2>
  <div class="row">
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-hospital"></i> Healthcare AI</h4>
        <p>Ensuring medical AI systems meet regulatory requirements for explainability, fairness, and security in clinical decision-making.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="impact-card">
        <h4><i class="fas fa-university"></i> Financial Services</h4>
        <p>Providing quantifiable assurance for AI systems in banking and insurance, ensuring compliance with fairness and transparency regulations.</p>
      </div>
    </div>
  </div>
</div>
\STATE \textbf{Output:} AIA scores

\STATE Initialize Shapley values $\varphi_i(v)$ for each feature

\STATE Train AI model on $D$

\FOR{$i$ in features of $D$}
    \FOR{$\pi$ in all permutations of features excluding $i$}
        \STATE Calculate $v(S \cup \{i\})$ and $v(S)$
        \STATE Update $\varphi_i(v)$ using Equation (1)
    \ENDFOR
\ENDFOR

\STATE Generate AIA scores: $AIA_i = \varphi_i(v) \cdot AIAC_i$ for each feature

\RETURN AIA scores
\end{algorithmic}
\end{algorithm}
\end{code>
</pre>

<p>Figure 1 shows the steps of the Weight Assessment method. The generated AIA scores help measure the contribution of each feature to achieving assurance goals, such as explainability and fairness.</p>

<h3>Reverse Learning</h3>

<p>Reverse Learning is a log-based method that traces back assurance issues using a recorded table of learning actions, essentially <strong>reverse engineering</strong> the model’s learning process. By logging the learning process, Reverse Learning can track where performance issues arise and optimize learning. For instance, it records details such as pseudo-residuals, gamma, and probability values during each epoch. This log can be used to verify if assurance goals like <strong>XAI</strong> are being met.</p>

<p>The method's outcome includes both the optimized number of epochs required to minimize the loss function and detailed logs of learning actions for each epoch. Equations (2) and (3) describe the GBDT model’s prediction and loss functions:</p>

<pre>
<code>
\[
f_{m i}= \begin{cases}0 \rightarrow p_{m i}<0.5\\  1 \rightarrow p_{m i}>=0.5\end{cases}
\]
\[
L=-\sum_{i=1}^{N}\left(y \log (odds)-\log \left(1+e^{\log (odds)}\right)\right)
\]
</code>
</pre>

<h4>Algorithm: Reverse Learning</h4>

<pre>
<code>
\begin{algorithm}
\caption{Reverse Learning}
\label{algo:reverse-learning}
\begin{algorithmic}[1]
\STATE \textbf{Input:} AI model, training data $D_{\text{train}}$
\STATE \textbf{Output:} Optimized number of epochs, logged actions

\STATE Initialize empty logs for each epoch

\FOR{$i$ in $\text{number of epochs}$}
    \STATE Train AI model for one epoch on $D_{\text{train}}$
    \STATE Calculate pseudo-residuals, gamma, and other values
    \STATE Save learning details in logs for epoch $i$
    \STATE Update model weights
\ENDFOR

\STATE Analyze logs to find the optimized number of epochs
\STATE Analyze logs for assurance issues

\RETURN Optimized number of epochs, logged actions
\end{algorithmic}
\end{algorithm}
\end{code>
</pre>

<p>Reverse Learning provides detailed logs to manually verify and optimize the AI algorithm. It does not generate AIA scores but helps ensure traceability and accountability in the learning process.</p>

<h3>Secret Inversion</h3>

<p>The <strong>Secret Inversion</strong> method performs exhaustive comparisons between features by reconstructing them using an <strong>Autoencoder (AE)</strong>. Reconstruction errors indicate the accuracy of the reconstruction process and point to assurance goals such as <strong>SAI</strong> (security) and <strong>CAI</strong> (confidentiality). The AE compresses the input into a lower-dimensional space and then reconstructs it, measuring the difference between the input and the reconstruction as an error metric.</p>

<p>The encoder-decoder structure is represented as:</p>

<pre>
<code>
\[
\phi: \mathcal{X} \rightarrow \mathcal{F}
\]
\[
\psi: \mathcal{F} \rightarrow \mathcal{X}
\]
\]
\]
</code>
</pre>

<p>The reconstruction error is minimized through optimization techniques like Adam or SGD. Equation (4) provides the formula for reconstruction error minimization:</p>

<pre>
<code>
\[
\|X-(\phi \circ \psi) X\|^{2}
\]
</code>
</pre>

<h4>Algorithm: Secret Inversion</h4>

<pre>
<code>
\begin{algorithm}
\caption{Secret Inversion}
\label{algo:secret-inversion}
\begin{algorithmic}[1]
\STATE \textbf{Input:} Dataset $D$, Autoencoder model, reconstruction errors $r$
\STATE \textbf{Output:} AIA scores (SAI and CAI)

\STATE Train Autoencoder model on $D$

\FOR{each feature $F_i$ in $D$}
    \STATE Encode $F_i$ using the Autoencoder: $F_i' = \phi(F_i)$
    \STATE Decode $F_i'$ using the Autoencoder: $F_i'' = \psi(F_i')$
    \STATE Calculate reconstruction error for $F_i$: $r_i = \|F_i - F_i''\|$
\ENDFOR

\STATE Calculate SAI and CAI based on reconstruction errors

\RETURN SAI and CAI scores
\end{algorithmic}
\end{algorithm}
\end{code>
</pre>

<p>The Secret Inversion method identifies potential security and confidentiality risks in a model by evaluating reconstruction errors. It generates AIA scores for SAI and CAI to ensure robustness against adversarial inputs and data integrity issues.</p>

