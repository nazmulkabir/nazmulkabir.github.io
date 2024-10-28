---
layout: page
title: DeepAg
description: Deep learning based precision farming
img: assets/img/Deepag.png
importance: 5
category: work
---

<h2>Outlier Detection in Agricultural Production Systems - DeepAg</h2>

<p>This section presents outlier detection (OD) methods using machine learning (ML) and deep learning (DL) models in Agricultural Production Systems (APS). The methodology involves unsupervised anomaly detection approaches, such as Isolation Forest, to identify outliers in the agricultural data. These techniques enable precision farming by detecting anomalies that may signify economic risks or operational inefficiencies.</p>

<h3>Isolation Forest</h3>

<p>The Isolation Forest algorithm is designed for unsupervised anomaly detection. It isolates outliers by constructing a binary tree structure where outliers are more likely to be isolated earlier in the process compared to normal data points. The key idea is that outliers require fewer splits to be isolated, leading to shorter path lengths in the trees. Figure 1 illustrates the Isolation Forest algorithm.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/Isolation_Forest.png" alt="Isolation Forest Method for OD" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 1: Isolation Forest Method for OD</em> (<a href="https://doi.org/10.1109/ICOIN.2021.9366416">Regaya et al., 2021</a>)</p>
        </div>
    </div>
</div>

<p>The Isolation Forest constructs multiple isolation trees, each of which is built using a random subset of data points and features. The algorithm assigns an anomaly score to each data point based on the number of splits required to isolate it. Figure 2 shows the DeepAg methodology, where economic indices (e.g., Crude Oil, Gold, Dow Jones, S&amp;P 500, VIX) are used as inputs for anomaly detection.</p>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/methods-deepag.png" alt="DeepAg Methodology" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 2: DeepAg Methodology</em> (<a href="https://doi.org/10.1109/ACCESS.2021.3056591">Gurrapu et al., 2021</a>)</p>
        </div>
    </div>
</div>

<h4>Algorithm: Isolation Forest for Outlier Detection</h4>

<pre>
<code>
\begin{algorithm}
\caption{Isolation Forest for Outlier Detection}
\label{algo:Isolation-Forest}
\begin{algorithmic}[1]
\STATE \textbf{Input:} Dataset $X$, number of trees $T$, sub-sampling size $S$
\STATE \textbf{Output:} Outlier scores for each data point

\STATE Initialize an empty set of isolation trees: $F = \{\}$

\FOR{$t$ in $1$ to $T$}
    \STATE Randomly select $S$ samples from $X$ without replacement to create a sub-sample $X_s$
    \STATE Create a new isolation tree $T_t$ using $X_s$ as follows:
        \STATE \hspace{10pt} If $X_s$ contains only one point or maximum depth is reached, create a leaf node with that point.
        \STATE \hspace{10pt} Otherwise, randomly select a feature $A$ from the remaining features.
        \STATE \hspace{10pt} Randomly select a split value $p$ for feature $A$ within its range in $X_s$.
        \STATE \hspace{10pt} Split $X_s$ into two subsets: $X_{\text{left}}$ containing points with $A \leq p$ and $X_{\text{right}}$ with $A > p$.
        \STATE \hspace{10pt} Create a non-leaf node with feature $A$ and split value $p$.
        \STATE \hspace{10pt} Recursively build the left subtree using $X_{\text{left}}$ and the right subtree using $X_{\text{right}}$.
    \STATE Add the newly created isolation tree $T_t$ to the set $F$
\ENDFOR

\STATE Compute the anomaly score for each data point in $X$ as follows:
\FOR{each data point $x$ in $X$}
    \STATE For each isolation tree $T_t$ in $F$, traverse the tree to find the depth $d_t(x)$ at which $x$ is isolated.
    \STATE Calculate the average depth across all trees: $D(x) = \frac{1}{T}\sum_{t=1}^{T} d_t(x)$
    \STATE Compute the anomaly score for each data point $x$: $S(x) = 2^{-\frac{D(x)}{c}}$, where $c$ is a normalizing factor.
\ENDFOR

\RETURN Anomaly scores for each data point
\end{algorithmic}
\end{algorithm}
</code>
</pre>

<h3>Anomaly Detection Thresholds and Contamination Rates</h3>

<p>The contamination rate is a key parameter in the Isolation Forest algorithm, which estimates the percentage of outliers in the dataset. It is typically determined using the <strong>Interquartile Range (IQR)</strong>, a statistical measure that describes the middle 50% of the data distribution. IQR is calculated as the difference between the third quartile (Q3) and the first quartile (Q1), as shown in Equation (1):</p>

<pre>
<code>
\[
\text{Interquartile Range} = Q3 - Q1
\]
</code>
</pre>

<div class="row">
    <div class="col-sm-12">
        <img src="Figures/IQR.png" alt="Interquartile Range Diagram" class="img-fluid rounded z-depth-1">
        <div class="caption">
            <p><em>Figure 3: Interquartile Range Diagram</em></p>
        </div>
    </div>
</div>

<p>The contamination rate helps estimate the anomaly threshold value, which is used to classify data points as outliers. Tables 1a and 1b present the contamination rates for daily and monthly financial indices using the IQR method.</p>

<pre>
<code>
\begin{table}[!ht]
\caption{Contamination Rates for Financial Indices using IQR}
\label{tab:iqr-combined}
\begin{subtable}{\textwidth}
  \caption{Daily Data Contamination (\%)}
  \begin{tabular}{|l|l|}
    \hline
    Financial Index & Contamination Rate \\
    \hline
    VIX & 6.559 \\
    \hline
    Gold & 5.382 \\
    \hline
    S\&P 500 & 6.008 \\
    \hline
    DOW & 6.125 \\
    \hline
    Crude Oil & 3.953 \\
    \hline
  \end{tabular}
\end{subtable}

\begin{subtable}{\textwidth}
  \caption{Monthly Data Contamination (\%)}
  \begin{tabular}{|l|l|}
    \hline
    Financial Index & Contamination Rate \\
    \hline
    VIX & 6.250 \\
    \hline
    Gold & 2.232 \\
    \hline
    S\&P 500 & 2.232 \\
    \hline
    DOW & 2.232 \\
    \hline
    Crude Oil & 6.250 \\
    \hline
  \end{tabular}
\end{subtable}
\end{table}
</code>
</pre>

<p>The anomaly score for each data point is computed based on the path length in the isolation trees, as described by Equation (2):</p>

<pre>
<code>
\[
s(x, m) = 2^{-E(h(x)) / c(m)}
\]
</code>
</pre>

<p>Finally, a threshold value <strong>T</strong> is selected using contamination rates to classify data points as outliers or normal, as defined in Equations (3) and (4):</p>

<pre>
<code>
\[
\text{If } S(x) < T, \text{ then } x \text{ is a normal data point.}
\]
\[
\text{If } S(x) \geq T, \text{ then } x \text{ is an outlier.}
\]
</code>
</pre>

<p>The detailed steps of the Isolation Forest for outlier detection in economic data are presented in Algorithm 1 above. This approach efficiently detects anomalies in high-dimensional datasets, making it suitable for APS data analysis.</p>
