---
layout: page
title: conda-forge/conda-smithy Contributions
---

<div style="text-align:center; margin-top:2rem; margin-bottom:2rem;">
<h1 style="margin-bottom:0.5rem;">conda-forge/conda-smithy Contributions</h1>
</div>

---

<div style="background:#f9fafb; padding:1.5rem; border-radius:12px; margin-bottom:2rem;">

<p><strong>PR #2435 – Add Podman support and SELinux handling to run_docker_build.sh template</strong><br>
Merged: Mar 2026</p>

<ul>
<li>Added automatic container runtime detection with Docker → Podman fallback</li>
<li>Introduced configurable runtime via <code>CONTAINER_RUNTIME</code> environment variable override</li>
<li>Replaced hardcoded Docker commands with a runtime-agnostic abstraction</li>
<li>Implemented rootless Podman permission fix using <code>podman unshare chown</code></li>
<li>Added SELinux-compatible volume labeling (<code>:z</code>) for enforcing environments</li>
<li>Preserved backward compatibility with existing Docker-based workflows</li>
<li>Incorporated multi-round maintainer feedback and added a news entry</li>
</ul>

<p>
<a href="https://github.com/conda-forge/conda-smithy/pull/2435"
   style="display:inline-block; padding:8px 14px; border-radius:8px;
   background:#eef2ff; text-decoration:none; font-weight:600;">
   View Pull Request
</a>
</p>

</div>
