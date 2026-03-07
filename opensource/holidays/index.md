---
layout: page
title: vacanza/holidays Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">vacanza/holidays Contributions</h1>
</div>

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #3178 – Add French Localization (l10n) Support for Gabon</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Set <code>default_language = "fr"</code> with support for <code>en_US</code> and <code>fr</code></li>
<li>Wrapped all holiday name literals using <code>gettext</code> (<code>tr()</code>) for localization</li>
<li>Added two complete <code>.po</code> localization catalogs (<code>fr</code> and <code>en_US</code>)</li>
<li>Used official French holiday names sourced from Gabonese government archives</li>
<li>Implemented multilingual tests (<code>test_l10n_default</code> and <code>test_l10n_en_us</code>)</li>
<li>Updated README language support table for Gabon</li>
<li>Passed 32 CI checks across Python 3.10–3.14 on macOS, Ubuntu, and Windows</li>
<li>Improved localization consistency for Francophone countries in the project</li>
</ul>

<p>
<a href="https://github.com/vacanza/holidays/pull/3178"
style="display:inline-block; padding:8px 14px; border-radius:8px;
background:#eef2ff; text-decoration:none; font-weight:600;">
View Pull Request
</a>
</p>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #3177 – Add French Localization (l10n) Support for Burkina Faso</strong><br>
Merged: Feb 2026</p>

<ul>
<li>Integrated <code>gettext</code> (<code>gettext as tr</code>) across all Burkina Faso holiday name literals</li>
<li>Set <code>en_BF</code> as default language with support for <code>en_US</code> and <code>fr</code></li>
<li>Added three complete <code>.po</code> localization catalogs (en_BF, en_US, fr)</li>
<li>Localized observed and estimated suffix labels (e.g., <code>(observed)</code>, <code>(estimated)</code>)</li>
<li>Implemented locale-aware spelling differences (Labor vs Labour)</li>
<li>Added comprehensive multilingual tests validating default, en_US, and French outputs</li>
<li>Updated README language table and CONTRIBUTORS attribution</li>
<li>Passed 32 CI checks and multi-maintainer review process before merge</li>
</ul>

<p>
<a href="https://github.com/vacanza/holidays/pull/3177"
style="display:inline-block; padding:8px 14px; border-radius:8px;
background:#eef2ff; text-decoration:none; font-weight:600;">
View Pull Request
</a>
</p>

</div>
