---
layout: page
title: AiiDA Core Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">

<h1 style="margin-bottom:0.5rem;">AiiDA Core Contributions</h1>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #7121 – Downgrade SQLite Lock Warning Level</strong><br>
Merged: Jan 2026</p>

<ul>
<li>Reduced log noise by changing expected SQLite lock logs from <code>WARNING</code> → <code>INFO</code></li>
<li>Preserved severity for genuine database issues</li>
<li>Improved observability across CI and production environments</li>
<li>Maintained full functional backward compatibility</li>
<li>Aligned logging behavior with real-world workflow expectations</li>
</ul>

<p>
<a href="https://github.com/aiidateam/aiida-core/pull/7121"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
