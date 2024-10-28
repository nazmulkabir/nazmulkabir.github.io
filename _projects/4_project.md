---
layout: page
title: MAA
description: Model Agnostic Assurance methods for AI solutions
img: assets/img/MAA.png
importance: 6
category: work
---

<h2>Model Agnostic Assurance Framework - ALSP</h2>

<p>This section introduces the <strong>ALSP</strong> framework for achieving quantifiable assurance goals, including <strong>XAI</strong> (Explainable AI), <strong>FAI</strong> (Fair AI), and <strong>SAI</strong> (Secure AI). The framework validates AI systems by providing quantifiable Assurance in AI (AIA) scores using a combination of data-driven and model-driven approaches. Specifically, ALSP optimizes models using a game theory approach and logs the actions of AI models to detect adversarial inputs, ensuring the datasets used for training are robust. To meet these assurance goals, ALSP employs three methods: <strong>Weight Assessment</strong>, <strong>Reverse Learning</strong>, and <strong>Secret Inversion</strong>, as depicted in Figure 1.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/ALSP.png" alt="Adversarial Logging Scoring Pipeline" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 1: Adversarial Logging Scoring Pipeline</em></p>
        </div>
    </div>
</div>

<h3>Weight Assessment</h3>

<p>Weight Assessment uses <strong>Game Theory</strong> to calculate <strong>Shapley values</strong> at every epoch of learning. The method provides AIA scores by assigning scores per data point, rather than aggregating them. For the Weight Assessment study, an Extreme Gradient Boosting Decision Tree (XGBDT) model was used as a baseline. Shapley values represent each feature's contribution to the overall prediction by modeling cooperation among features (players) in a game setting.</p>

<p>The Shapley values are calculated by averaging the marginal contribution of a feature across all possible permutations, as shown in Equation (1):</p>

<pre>
<code>
\[
\varphi_{i}(v)=\frac{1}{n} \sum_{S \subseteq N \backslash\{i\}}\left(\begin{array}{c}
n-1 \\
|S|
\end{array}\right)^{-1}(v(S \cup\{i\})-v(S))
\]
</code>
</pre>

<p>The resulting Shapley values are combined with assurance labels (AIAC) assigned by domain experts to calculate AIA scores for each feature. These assurance labels relate to goals like explainability or fairness, ensuring that features relevant to assurance goals are adequately weighted in the model.</p>

<h4>Algorithm: Weight Assessment</h4>

<pre>
<code>
\begin{algorithm}
\caption{Weight Assessment}
\label{algo:weight-assessment}
\begin{algorithmic}[1]
\STATE \textbf{Input:} AI model, dataset $D$, assurance labels $AIAC$
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

