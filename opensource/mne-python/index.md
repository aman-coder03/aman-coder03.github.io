---
layout: page
title: mne-python Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">

<h1 style="margin-bottom:0.5rem;">mne-python Contributions</h1>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #13710 – Add Epoch Quality Example(How-To Guide for Identifying Artifactual Epochs)</strong><br>
Merged: Apr 2026</p>

<ul>
<li>Added a Sphinx-gallery how-to example demonstrating per-epoch outlier scoring using peak-to-peak amplitude, variance, and kurtosis — inspired by FASTER (Nolan et al., 2010) and Delorme et al. (2007)</li>
<li>Used the EEGBCI dataset with two thresholds (0.6 and 0.3) to demonstrate the quality-quantity trade-off, with epoch plots at each threshold to make artifacts visually prominent</li>
<li>Structured as a diataxis-aligned how-to guide per maintainer feedback, assuming prior MNE knowledge and leading with the task goal</li>
<li>Added footcite references to doc/references.bib following MNE documentation standards</li>
<li>Incorporated multi-round feedback from three reviewers (larsoner, tsbinns, CarinaFo), iterating on dataset choice, threshold selection, channel visibility, and example structure</li>
</ul>

<p>
<a href="https://github.com/mne-tools/mne-python/pull/13710"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>
   
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #13729 – Add Python–R Interoperability Example using rpy2</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Added a Sphinx-gallery example demonstrating a mass-univariate t-test using Python and R (via rpy2)</li>
<li>Showed full interoperability: NumPy → R conversion, executing R functions, retrieving results back into Python</li>
<li>Integrated rpy2 into documentation dependencies and updated CI to install R</li>
<li>Resolved cross-platform build issues via CircleCI configuration (R + system libraries)</li>
<li>Incorporated maintainer feedback: moved to stats module, improved ROI selection and ERP window, expanded rpy2 explanations</li>
<li>Ensured successful documentation build with all CI checks passing</li>
</ul>

<p>
<a href="https://github.com/mne-tools/mne-python/pull/13729"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #13570 – Add Optional Channel Name Overlay to plot_alignment</strong><br>
Merged: Feb 2026</p>

<ul>
<li>Added optional <code>show_channel_names</code> parameter to <code>plot_alignment</code></li>
<li>Implemented channel label overlay at sensor coordinates in 3D alignment view</li>
<li>Reused existing 3D plotting infrastructure for text rendering</li>
<li>Updated tutorial example to showcase the feature in rendered documentation</li>
<li>Maintained full backward compatibility (default behavior unchanged)</li>
</ul>

<p>
<a href="https://github.com/mne-tools/mne-python/pull/13570"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
