---
layout: page
title: matplotlib/matplotlib Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">matplotlib/matplotlib Contributions</h1>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #31278 – Fix clabel manual argument not accepting unit-typed coordinates</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Added <code>self.axes.convert_xunits(x)</code> and <code>self.axes.convert_yunits(y)</code> calls in <code>add_label_near()</code> in <code>contour.py</code> before applying the transform, consistent with the pattern already used in <code>_base.py</code></li>
<li>The fix is a no-op when no unit converter is registered, so non-unit axes are completely unaffected</li>
<li>Filled in the existing <code>test_clabel</code> stub in <code>test_datetime.py</code> with a real test that verifies the label is placed correctly, asserting on both the label text and position</li>
</ul>

<p>
<a href="https://github.com/matplotlib/matplotlib/pull/31278"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
