---
layout: page
title: braindecode/braindecode Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">braindecode/braindecode Contributions</h1>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #941 – Add mapping, preload, picks, drop_bad_windows, and descriptions support to create_from_mne_epochs</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Implemented <code>mapping</code> to remap integer event codes to target values, consistent with the raw-based API</li>
<li>Forwarded <code>preload</code> and <code>picks</code> to the internal <code>mne.Epochs</code> call for memory and channel control</li>
<li>Introduced <code>drop_bad_windows</code> to conditionally call <code>.drop_bad()</code> on resulting epochs</li>
<li>Supported <code>descriptions</code> with length validation to attach per-dataset metadata, matching <code>create_from_mne_raw()</code> behavior</li>
<li>All parameters default to <code>None</code>/<code>False</code>/<code>True</code> preserving full backward compatibility</li>
<li>Covered all five new parameters with parametrized pytest tests using shared fixtures</li>
</ul>

<p>
<a href="https://github.com/braindecode/braindecode/pull/941"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
