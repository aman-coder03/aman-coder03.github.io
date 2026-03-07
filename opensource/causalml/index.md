---
layout: page
title: uber/causalml Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">uber/causalml Contributions</h1>
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
