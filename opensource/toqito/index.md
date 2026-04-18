---
layout: page
title: vprusso/toqito Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">vprusso/toqito Contributions</h1>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">
<p><strong>PR #1390 – Parameterize random_psd_operator with Wishart Distribution Option</strong><br>
Merged: Apr 2026</p>
<ul>
<li>Added <code>distribution: Literal["uniform", "wishart"]</code> parameter to <code>random_psd_operator</code> with full backward compatibility</li>
<li>Implemented Wishart sampling with correct complex normalization (<code>/sqrt(2)</code>) following Goodman (1963)</li>
<li>Added optional <code>scale</code> (PSD scale matrix) and <code>num_degrees</code> (degrees of freedom) parameters for full Wishart parameterization</li>
<li>Added <code>np.asarray</code> coercion for <code>scale</code> to gracefully handle list/tuple input</li>
<li>Added validation for <code>scale</code> shape and positive semidefiniteness, and integer/positivity checks for <code>num_degrees</code></li>
<li>Added <code>UserWarning</code> for rank-deficient Wishart matrices (<code>num_degrees &lt; dim</code>) and ignored Wishart params on uniform path</li>
<li>Updated docstring with <code>Raises</code> section, Google-style format, and mkdocs-compatible examples</li>
</ul>
<p>
<a href="https://github.com/vprusso/toqito/pull/1390"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">
<p><strong>PR #1391 – Ensure partial_trace Raises ValueError for Invalid Parameters</strong><br>
Merged: Apr 2026</p>
<ul>
<li>Added explicit square matrix check with clear <code>ValueError: input_mat must be a 2D square matrix</code></li>
<li>Added <code>np.prod(dim) != n</code> validation to catch mismatched subsystem dimensions</li>
<li>Added out-of-bounds and negative index validation for <code>sys</code> subsystem indices</li>
<li>Broadened <code>dim</code> and <code>sys</code> type support to accept <code>list</code>, <code>tuple</code>, and <code>np.ndarray</code> using <code>np.asarray</code></li>
<li>Updated type annotations and docstring <code>Raises</code> section to document all <code>ValueError</code> conditions</li>
<li>Replaced silent NumPy failures and cryptic <code>IndexError</code> crashes with actionable error messages</li>
</ul>
<p>
<a href="https://github.com/vprusso/toqito/pull/1391"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>
</div>

---

