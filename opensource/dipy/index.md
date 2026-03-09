---
layout: page
title: dipy/dipy Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">

<h1 style="margin-bottom:0.5rem;">dipy/dipy Contributions</h1>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">
<p><strong>PR #3783 – Fix Figure Canvas Not Cleared in Simulation Tutorials</strong><br>
Merged: Mar 2026</p>
<ul>
<li>Identified simulation tutorials missing explicit <code>plt.figure()</code> calls before plotting in sphinx-gallery builds</li>
<li>Replaced bare <code>plt.plot()</code> calls with <code>fig, ax = plt.subplots()</code> (object-oriented API) in <code>simulate_dki.py</code> and <code>simulate_multi_tensor.py</code></li>
<li>Built documentation locally on Windows using meson-python and MSVC, verifying both tutorials executed successfully</li>
<li>Confirmed clean, separate figure generation with no canvas overlap in generated documentation</li>
<li>Documentation-only fix with no functional behavior changes</li>
</ul>
<p>
<a href="https://github.com/dipy/dipy/pull/3783"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #3780 – Fix numpydoc Validation Issues in fetcher.py</strong><br>
Merged: Feb 2026</p>

<ul>
<li>Standardized docstrings in <code>dipy/data/fetcher.py</code> to follow numpydoc conventions</li>
<li>Corrected <code>Returns</code> section formatting and removed duplicate entries</li>
<li>Updated type annotations from <code>string</code> to <code>Path</code> where appropriate</li>
<li>Improved docstring clarity and ensured proper Sphinx rendering</li>
<li>Maintained full backward compatibility (documentation-only change)</li>
</ul>

<p>
<a href="https://github.com/dipy/dipy/pull/3780"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
