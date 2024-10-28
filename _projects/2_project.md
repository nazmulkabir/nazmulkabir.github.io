---
layout: page
title: DeepH2O
description: HCAE and TGCN models for detecting cyber-attacks in water distribution systems
img: assets/img/DeepH2O.png
importance: 2
category: work
giscus_comments: true
---

<h2>DeepH2O: Hybrid Cyber-Attack Detection in Water Distribution Systems</h2>

<p>Water Distribution Systems (WDS) are critical infrastructure, often vulnerable to various cyber-physical attacks. <strong>DeepH2O</strong> leverages cutting-edge machine learning models—<strong>High Confidence AutoEncoder (HCAE)</strong> and <strong>Temporal Graph Convolutional Networks (TGCN)</strong>—to detect these cyber-attacks with minimal false positives. The HCAE architecture is designed to handle non-deterministic training issues common in traditional AutoEncoders (AEs), and TGCN captures the temporal and spatial dependencies within WDS sensor data, improving the detection performance. This project aims to provide a robust framework for anomaly detection, ensuring high accuracy with minimal maintenance costs.</p>

<h3>AutoEncoder (AE) for Anomaly Detection</h3>

<p>AutoEncoders have long been used for <strong>dimensionality reduction</strong> and <strong>feature learning</strong>. The AE architecture used in this project follows a basic structure consisting of an <strong>encoder</strong> and <strong>decoder</strong> pair. The encoder compresses input data into a lower-dimensional feature space, while the decoder attempts to reconstruct the original input from this compressed representation.</p>

<p>The goal of this architecture is to minimize reconstruction error, which is indicative of how well the model has captured the underlying data structure. Mathematically, the encoder-decoder system can be described as:</p>

<pre>
<code>
\[
\phi: \mathcal{X} \rightarrow \mathcal{F}
\]
\[
\psi: \mathcal{F} \rightarrow \mathcal{X}
\]
\[
\phi, \psi=\underset{\phi, \psi}{\arg \min }\|\mathcal{X}-(\psi \circ \phi) \mathcal{X}\|^{2}
\]
</code>
</pre>

<p>The reconstruction loss is given by:</p>

<pre>
<code>
\[
\mathcal{L}\left(\mathbf{x}, \mathbf{x}^{\prime}\right)=\left\|\mathbf{x}-\mathbf{x}^{\prime}\right\|^{2}
\]
</code>
</pre>

<p>This standard AE setup provides the baseline for anomaly detection, where higher reconstruction errors typically indicate anomalies or attacks.</p>

<h3>High Confidence AutoEncoder (HCAE)</h3>

<p>In water distribution systems, false positives from anomaly detection models can result in costly maintenance operations. <strong>HCAE</strong> improves upon the traditional AE by incorporating <strong>deterministic learning</strong> through a series of constraints that ensure the model consistently learns important features across multiple training sessions.</p>

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
        <img src="img/ae/300_dpi_hcae.jpg" alt="Fully Connected ANN-based Autoencoder for WDS" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 1: Fully Connected ANN-based Autoencoder for WDS</em></p>
        </div>
    </div>
</div>

<h3>Attack Detection Workflow in HCAE</h3>

<p>The <strong>HCAE</strong> model's workflow involves two key stages: model development and attack detection. The model is trained on normal WDS data, with reconstruction errors minimized during training using the <strong>Adam optimizer</strong>. Once trained, the model detects anomalies in new data based on reconstruction errors that exceed a threshold, $\theta_{th}$, determined empirically.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="img/ae/HCAE-stages.png" alt="HCAE Model Development and Attack Detection Workflow" class="img-fluid rounded z-depth-1">
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
