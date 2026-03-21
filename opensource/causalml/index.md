---
layout: page
title: uber/causalml Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">uber/causalml Contributions</h1>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #887 – Add Rank-weighted Average Treatment Effect (RATE) Metric</strong><br>
Merged: Mar 2026</p>
<ul>
<li>Added <code>causalml/metrics/rate.py</code> with three public functions — <code>get_toc()</code>, <code>rate_score()</code>, and <code>plot_toc()</code> — following the exact same API conventions as <code>get_qini</code> / <code>qini_score</code> / <code>plot_qini</code></li>
<li><code>get_toc()</code> computes the Targeting Operator Characteristic curve via O(n) cumulative sums; <code>rate_score()</code> computes the RATE scalar with AUTOC (1/q) or Qini (q) weighting; <code>plot_toc()</code> visualizes the TOC curve</li>
<li>Supported both oracle mode (simulated <code>tau</code>) and observed RCT mode (<code>y</code> + <code>w</code>); fixed normalize division-by-zero by using <code>max(|TOC|)</code> instead of <code>TOC(1)</code>; added <code>logger.warning</code> for observed-outcome fallback</li>
<li>Added 20 unit tests in <code>tests/test_rate.py</code>; addressed all blocking and non-blocking review comments across two review rounds; passed black and pre-commit clean</li>
<li>Implementation verified correct against the Yadlowsky et al. (2021) paper and the grf R package reference by the maintainer</li>
</ul>
<p>
<a href="https://github.com/uber/causalml/pull/887"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">
  
<p><strong>PR #860 – Add Native NaN Support for UpliftTree and UpliftRandomForest</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Added native NaN routing logic to each candidate split, evaluating both left/right directions and learning the optimal routing per node — consistent with scikit-learn's decision tree behavior</li>
<li>Stored the learned NaN routing in each <code>DecisionTree</code> node and applied it consistently during training, pruning, filling, and prediction</li>
<li>Guarded all <code>np.isnan()</code> calls with <code>np.issubdtype(..., np.number)</code> to prevent <code>TypeError</code> on string/categorical columns</li>
<li>Added NaN-aware percentile calculation by filtering out NaN values before computing split thresholds</li>
<li>Added two targeted tests: one for NaN values in numeric columns, one for <code>None</code> values in object-dtype columns</li>
</ul>

<p>
<a href="https://github.com/uber/causalml/pull/860"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
