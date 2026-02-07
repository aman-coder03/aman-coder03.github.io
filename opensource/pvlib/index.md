---
layout: page
title: pvlib Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">

<h1 style="margin-bottom:0.5rem;">pvlib Contributions</h1>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #2680 – Fix Swapped Reference Numbering in get_bsrn</strong><br>
Merged: Feb 2026 · Milestone: v0.15.1</p>

<ul>
<li>Corrected interchanged reference labels in <code>pvlib.iotools.get_bsrn</code> docstring</li>
<li>Ensured consistency with related BSRN utilities (e.g., <code>read_bsrn</code>)</li>
<li>Verified proper rendering in the <em>latest</em> documentation build</li>
<li>Scoped strictly to documentation — no functional or API changes</li>
<li>Improved citation clarity in scientific documentation workflows</li>
</ul>

<p>
<a href="https://github.com/pvlib/pvlib-python/pull/2680"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #2648 – Use ValueError Instead of IndexError in _degrees_to_index</strong><br>
Merged: Feb 2026 · Milestone: v0.15.1</p>

<ul>
<li>Replaced incorrect <code>IndexError</code> with <code>ValueError</code> for invalid latitude/longitude inputs</li>
<li>Aligned exception semantics with Python and NumPy conventions</li>
<li>Updated affected unit tests and related clearsky tests accordingly</li>
<li>Resolved CI failures and ensured full test suite pass before merge</li>
<li>Improved API correctness without altering functional behavior</li>
</ul>

<p>
<a href="https://github.com/pvlib/pvlib-python/pull/2648"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #2646 – Fix ZeroDivisionError in transformer.simple_efficiency</strong><br>
Merged: Feb 2026 · Milestone: v0.15.1</p>

<ul>
<li>Resolved a <code>ZeroDivisionError</code> triggered when <code>load_loss = 0</code> (physically valid transformer edge case)</li>
<li>Reformulated the quadratic efficiency expression into a numerically stable form</li>
<li>Preserved existing behavior for <code>load_loss &gt; 0</code> to maintain backward compatibility</li>
<li>Added targeted unit test validating linear-limit behavior:
    <code>P_out = P_in − L_no_load × P_nom</code></li>
<li>Updated release notes and aligned documentation with maintainer guidance</li>
</ul>

<p>
<a href="https://github.com/pvlib/pvlib-python/pull/2646"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #2622 – Documentation Fix</strong><br>
Merged: Dec 2025</p>

<ul>
<li>Corrected contributor attribution typo in release notes</li>
<li>Restored broken documentation links</li>
<li>Maintained release documentation standards</li>
</ul>

<p>
<a href="https://github.com/pvlib/pvlib-python/pull/2622"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
