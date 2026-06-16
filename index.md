
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Aman Srivastava — Software Dev | AI/ML | Data Science</title>
<meta name="description" content="Aman Srivastava — Computer Science undergraduate specializing in AI/ML, Data Science, and Software Development." />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet" />
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg:       #000000;
    --bg-2:     #080808;
    --bg-card:  #0d0d0d;
    --border:   #1a1a1a;
    --border-2: #242424;
    --text:     #f0f0f0;
    --text-2:   #a0a0a0;
    --text-3:   #606060;
    --accent:   #a3e635;
    --accent-d: #84cc16;
    --accent-glow: rgba(163,230,53,0.15);
    --font-display: 'Space Grotesk', sans-serif;
    --font-body:    'Inter', sans-serif;
    --font-mono:    'JetBrains Mono', monospace;
    --radius:   14px;
    --radius-sm: 8px;
    --transition: 0.22s cubic-bezier(0.4,0,0.2,1);
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--font-body);
    font-size: 15px;
    line-height: 1.7;
    -webkit-font-smoothing: antialiased;
    overflow-x: hidden;
  }

  /* ── SCROLLBAR ── */
  ::-webkit-scrollbar { width: 4px; }
  ::-webkit-scrollbar-track { background: var(--bg); }
  ::-webkit-scrollbar-thumb { background: var(--border-2); border-radius: 2px; }

  /* ── LAYOUT ── */
  .shell {
    display: grid;
    grid-template-columns: 280px 1fr;
    min-height: 100vh;
    max-width: 1280px;
    margin: 0 auto;
  }

  /* ── SIDEBAR ── */
  .sidebar {
    position: sticky;
    top: 0;
    height: 100vh;
    padding: 3rem 2rem 3rem 2.5rem;
    display: flex;
    flex-direction: column;
    gap: 0;
    border-right: 1px solid var(--border);
    overflow-y: auto;
  }

  .sidebar-top { margin-bottom: auto; }

  .avatar-wrap {
    width: 72px;
    height: 72px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--accent) 0%, #22d3ee 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: var(--font-display);
    font-weight: 700;
    font-size: 1.6rem;
    color: #000;
    margin-bottom: 1.4rem;
    flex-shrink: 0;
    box-shadow: 0 0 0 3px var(--bg), 0 0 0 4px var(--border-2);
  }

  .sidebar-name {
    font-family: var(--font-display);
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.02em;
    line-height: 1.2;
    margin-bottom: 0.3rem;
  }

  .sidebar-role {
    font-size: 0.78rem;
    color: var(--accent);
    font-family: var(--font-mono);
    font-weight: 500;
    letter-spacing: 0.04em;
    margin-bottom: 0.4rem;
  }

  .sidebar-loc {
    font-size: 0.8rem;
    color: var(--text-3);
    margin-bottom: 1.8rem;
    display: flex;
    align-items: center;
    gap: 0.3rem;
  }

  .nav-label {
    font-size: 0.68rem;
    font-weight: 600;
    letter-spacing: 0.12em;
    color: var(--text-3);
    text-transform: uppercase;
    margin-bottom: 0.6rem;
    margin-top: 1.8rem;
  }

  .nav-links { list-style: none; display: flex; flex-direction: column; gap: 0.1rem; }

  .nav-links a {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    padding: 0.45rem 0.7rem;
    border-radius: var(--radius-sm);
    color: var(--text-2);
    text-decoration: none;
    font-size: 0.85rem;
    font-weight: 500;
    transition: color var(--transition), background var(--transition);
  }
  .nav-links a:hover, .nav-links a.active {
    color: var(--text);
    background: var(--border);
  }
  .nav-links a .dot {
    width: 5px; height: 5px;
    border-radius: 50%;
    background: var(--text-3);
    flex-shrink: 0;
    transition: background var(--transition);
  }
  .nav-links a:hover .dot, .nav-links a.active .dot { background: var(--accent); }

  .sidebar-social {
    display: flex;
    gap: 0.6rem;
    margin-top: 2rem;
    padding-top: 1.8rem;
    border-top: 1px solid var(--border);
  }

  .social-btn {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 36px; height: 36px;
    border-radius: var(--radius-sm);
    border: 1px solid var(--border-2);
    background: transparent;
    color: var(--text-3);
    text-decoration: none;
    font-size: 0.9rem;
    transition: all var(--transition);
  }
  .social-btn:hover {
    border-color: var(--accent);
    color: var(--accent);
    background: var(--accent-glow);
  }

  /* ── MAIN CONTENT ── */
  main {
    padding: 5rem 4rem 6rem 4rem;
    max-width: 860px;
  }

  /* ── SECTION ── */
  section { margin-bottom: 6rem; }

  .section-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    font-family: var(--font-mono);
    font-size: 0.7rem;
    font-weight: 500;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 1.2rem;
  }
  .section-eyebrow::before {
    content: '';
    display: block;
    width: 20px; height: 1px;
    background: var(--accent);
  }

  .section-title {
    font-family: var(--font-display);
    font-size: 2rem;
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.03em;
    line-height: 1.15;
    margin-bottom: 2.5rem;
  }

  /* ── HERO ── */
  #hero { margin-bottom: 5rem; }

  .hero-tag {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.3rem 0.8rem;
    border-radius: 999px;
    border: 1px solid var(--border-2);
    font-size: 0.75rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    margin-bottom: 2rem;
  }
  .hero-tag .pulse {
    width: 7px; height: 7px;
    border-radius: 50%;
    background: var(--accent);
    animation: pulse 2s ease-in-out infinite;
  }
  @keyframes pulse {
    0%,100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.4; transform: scale(0.7); }
  }

  .hero-name {
    font-family: var(--font-display);
    font-size: clamp(3rem, 6vw, 4.5rem);
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.04em;
    line-height: 1.05;
    margin-bottom: 0.6rem;
  }
  .hero-name .cursor {
    display: inline-block;
    width: 3px;
    height: 0.85em;
    background: var(--accent);
    margin-left: 4px;
    vertical-align: middle;
    border-radius: 2px;
    animation: blink 1.1s step-end infinite;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  .hero-sub {
    font-family: var(--font-display);
    font-size: clamp(1rem, 2.5vw, 1.35rem);
    color: var(--text-2);
    font-weight: 400;
    letter-spacing: -0.01em;
    margin-bottom: 0.5rem;
  }

  .hero-loc {
    font-size: 0.85rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    margin-bottom: 2.5rem;
    display: flex;
    align-items: center;
    gap: 0.4rem;
  }

  .hero-ctas { display: flex; gap: 0.8rem; flex-wrap: wrap; }

  .btn-primary {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.65rem 1.3rem;
    border-radius: var(--radius-sm);
    background: var(--accent);
    color: #000;
    font-weight: 600;
    font-size: 0.85rem;
    font-family: var(--font-display);
    text-decoration: none;
    transition: all var(--transition);
    letter-spacing: -0.01em;
  }
  .btn-primary:hover { background: var(--accent-d); transform: translateY(-1px); }

  .btn-ghost {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    padding: 0.65rem 1.3rem;
    border-radius: var(--radius-sm);
    background: transparent;
    border: 1px solid var(--border-2);
    color: var(--text-2);
    font-weight: 500;
    font-size: 0.85rem;
    font-family: var(--font-display);
    text-decoration: none;
    transition: all var(--transition);
  }
  .btn-ghost:hover { border-color: var(--text-3); color: var(--text); background: var(--border); }

  /* ── ABOUT ── */
  .about-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 2rem 2.2rem;
  }
  .about-card p {
    color: var(--text-2);
    line-height: 1.8;
    font-size: 0.925rem;
    margin-bottom: 1.1rem;
  }
  .about-card p:last-child { margin-bottom: 0; }
  .about-card strong { color: var(--text); font-weight: 600; }

  /* ── EXPERIENCE ── */
  .exp-list { display: flex; flex-direction: column; gap: 0; }

  .exp-item {
    display: grid;
    grid-template-columns: 20px 1fr;
    gap: 0 1.5rem;
  }

  .exp-timeline {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 0.35rem;
  }
  .exp-dot {
    width: 10px; height: 10px;
    border-radius: 50%;
    border: 2px solid var(--accent);
    background: var(--bg);
    flex-shrink: 0;
    position: relative;
    z-index: 1;
  }
  .exp-line {
    flex: 1;
    width: 1px;
    background: var(--border-2);
    margin-top: 4px;
    min-height: 2rem;
  }
  .exp-item:last-child .exp-line { display: none; }

  .exp-body {
    padding-bottom: 2.5rem;
  }

  .exp-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.6rem 1.8rem;
    transition: border-color var(--transition), transform var(--transition);
    cursor: default;
  }
  .exp-card:hover {
    border-color: var(--border-2);
    transform: translateY(-2px);
  }

  .exp-header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 1rem;
    margin-bottom: 0.2rem;
  }

  .exp-company {
    font-family: var(--font-display);
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.02em;
  }

  .exp-location {
    font-size: 0.72rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    padding: 0.2rem 0.6rem;
    border: 1px solid var(--border-2);
    border-radius: 999px;
    white-space: nowrap;
    flex-shrink: 0;
  }

  .exp-role {
    font-size: 0.85rem;
    color: var(--accent);
    font-weight: 500;
    margin-bottom: 0.25rem;
  }

  .exp-date {
    font-size: 0.75rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    margin-bottom: 1.1rem;
  }

  .exp-bullets {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 0.55rem;
  }
  .exp-bullets li {
    font-size: 0.855rem;
    color: var(--text-2);
    line-height: 1.65;
    padding-left: 1.1rem;
    position: relative;
  }
  .exp-bullets li::before {
    content: '→';
    position: absolute;
    left: 0;
    color: var(--accent);
    font-size: 0.75rem;
    top: 0.05em;
  }
  .exp-bullets li strong { color: var(--text); font-weight: 600; }

  /* ── PROJECTS ── */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
  }

  .proj-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.5rem 1.6rem;
    display: flex;
    flex-direction: column;
    gap: 0.7rem;
    transition: border-color var(--transition), transform var(--transition), box-shadow var(--transition);
    cursor: default;
    position: relative;
    overflow: hidden;
  }
  .proj-card::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(circle at top left, var(--accent-glow) 0%, transparent 65%);
    opacity: 0;
    transition: opacity var(--transition);
  }
  .proj-card:hover {
    border-color: var(--border-2);
    transform: translateY(-3px);
    box-shadow: 0 12px 40px rgba(0,0,0,0.5);
  }
  .proj-card:hover::before { opacity: 1; }

  .proj-icon {
    font-size: 1.3rem;
    margin-bottom: 0.1rem;
  }

  .proj-name {
    font-family: var(--font-display);
    font-size: 0.98rem;
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.02em;
    line-height: 1.3;
  }

  .proj-bullets {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 0.45rem;
    flex: 1;
  }
  .proj-bullets li {
    font-size: 0.8rem;
    color: var(--text-2);
    line-height: 1.6;
    padding-left: 1rem;
    position: relative;
  }
  .proj-bullets li::before {
    content: '·';
    position: absolute;
    left: 0.25rem;
    color: var(--accent);
    font-weight: 700;
  }
  .proj-bullets li strong { color: var(--text); font-weight: 600; }

  /* ── EDUCATION ── */
  .edu-grid { display: flex; flex-direction: column; gap: 1rem; }
  .edu-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.5rem 1.8rem;
    display: flex;
    align-items: flex-start;
    gap: 1.2rem;
    transition: border-color var(--transition);
  }
  .edu-card:hover { border-color: var(--border-2); }
  .edu-icon {
    width: 42px; height: 42px;
    border-radius: 10px;
    background: var(--border);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.2rem;
    flex-shrink: 0;
  }
  .edu-inst {
    font-family: var(--font-display);
    font-size: 0.98rem;
    font-weight: 700;
    color: var(--text);
    letter-spacing: -0.02em;
    margin-bottom: 0.15rem;
  }
  .edu-degree {
    font-size: 0.82rem;
    color: var(--accent);
    font-weight: 500;
    margin-bottom: 0.1rem;
  }
  .edu-meta {
    font-size: 0.75rem;
    color: var(--text-3);
    font-family: var(--font-mono);
  }

  /* ── ACHIEVEMENTS ── */
  .ach-grid { display: flex; flex-direction: column; gap: 0.8rem; }
  .ach-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.2rem 1.6rem;
    display: flex;
    align-items: center;
    gap: 1rem;
    transition: all var(--transition);
  }
  .ach-card:hover { border-color: var(--accent); background: rgba(163,230,53,0.03); }
  .ach-badge {
    width: 38px; height: 38px;
    border-radius: 9px;
    background: var(--accent-glow);
    border: 1px solid rgba(163,230,53,0.2);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.1rem;
    flex-shrink: 0;
  }
  .ach-title {
    font-size: 0.85rem;
    font-weight: 600;
    color: var(--text);
    font-family: var(--font-display);
  }
  .ach-desc {
    font-size: 0.78rem;
    color: var(--text-3);
    margin-top: 0.1rem;
  }

  /* ── CERTIFICATIONS ── */
  .cert-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 0.75rem;
  }
  .cert-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius-sm);
    padding: 0.9rem 1.1rem;
    display: flex;
    align-items: flex-start;
    gap: 0.7rem;
    transition: all var(--transition);
  }
  .cert-card:hover { border-color: var(--border-2); }
  .cert-dot {
    width: 7px; height: 7px;
    border-radius: 50%;
    background: var(--accent);
    margin-top: 0.45rem;
    flex-shrink: 0;
  }
  .cert-name {
    font-size: 0.8rem;
    font-weight: 600;
    color: var(--text);
    line-height: 1.4;
  }
  .cert-issuer {
    font-size: 0.72rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    margin-top: 0.15rem;
  }

  /* ── OPEN SOURCE ── */
  .os-hero {
    background: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 2rem 2.2rem;
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
    gap: 2rem;
  }
  .os-stat {
    text-align: center;
    flex-shrink: 0;
  }
  .os-number {
    font-family: var(--font-display);
    font-size: 2.8rem;
    font-weight: 700;
    color: var(--accent);
    letter-spacing: -0.05em;
    line-height: 1;
  }
  .os-label {
    font-size: 0.72rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    margin-top: 0.2rem;
    text-transform: uppercase;
    letter-spacing: 0.08em;
  }
  .os-divider { width: 1px; height: 60px; background: var(--border-2); flex-shrink: 0; }
  .os-desc { font-size: 0.9rem; color: var(--text-2); line-height: 1.7; }
  .os-desc strong { color: var(--text); font-weight: 600; }

  .os-ecosystems {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 1.2rem;
  }
  .eco-tag {
    padding: 0.3rem 0.8rem;
    border-radius: 999px;
    border: 1px solid var(--border-2);
    font-size: 0.73rem;
    color: var(--text-2);
    font-family: var(--font-mono);
    background: var(--bg-card);
    transition: all var(--transition);
  }
  .eco-tag:hover { border-color: var(--accent); color: var(--accent); }

  .os-link {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    margin-top: 1.5rem;
    color: var(--accent);
    font-size: 0.82rem;
    font-weight: 600;
    text-decoration: none;
    font-family: var(--font-mono);
    transition: gap var(--transition);
  }
  .os-link:hover { gap: 0.8rem; }

  /* ── FADE IN ANIMATION ── */
  .fade-in {
    opacity: 0;
    transform: translateY(18px);
    transition: opacity 0.55s cubic-bezier(0.4,0,0.2,1), transform 0.55s cubic-bezier(0.4,0,0.2,1);
  }
  .fade-in.visible { opacity: 1; transform: none; }

  /* ── MOBILE NAV ── */
  .mobile-nav {
    display: none;
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(0,0,0,0.85);
    backdrop-filter: blur(16px);
    -webkit-backdrop-filter: blur(16px);
    border-bottom: 1px solid var(--border);
    padding: 0.9rem 1.2rem;
    align-items: center;
    justify-content: space-between;
  }
  .mobile-name {
    font-family: var(--font-display);
    font-size: 1rem;
    font-weight: 700;
    color: var(--text);
  }
  .hamburger {
    background: none;
    border: none;
    color: var(--text-2);
    cursor: pointer;
    padding: 4px;
    font-size: 1.1rem;
    display: flex;
    flex-direction: column;
    gap: 5px;
  }
  .hamburger span {
    display: block;
    width: 22px; height: 2px;
    background: currentColor;
    border-radius: 1px;
    transition: all var(--transition);
  }
  .mobile-drawer {
    display: none;
    position: fixed;
    top: 0; left: 0; right: 0; bottom: 0;
    background: rgba(0,0,0,0.95);
    z-index: 200;
    padding: 2rem 1.5rem;
    flex-direction: column;
  }
  .mobile-drawer.open { display: flex; }
  .drawer-close {
    align-self: flex-end;
    background: none;
    border: none;
    color: var(--text-2);
    font-size: 1.5rem;
    cursor: pointer;
    margin-bottom: 2rem;
  }
  .drawer-nav { display: flex; flex-direction: column; gap: 0.3rem; }
  .drawer-nav a {
    padding: 0.8rem 0.5rem;
    color: var(--text-2);
    text-decoration: none;
    font-size: 1.1rem;
    font-family: var(--font-display);
    font-weight: 500;
    border-bottom: 1px solid var(--border);
    transition: color var(--transition);
  }
  .drawer-nav a:hover { color: var(--accent); }

  /* ── RESPONSIVE ── */
  @media (max-width: 1024px) {
    .shell { grid-template-columns: 1fr; }
    .sidebar { display: none; }
    .mobile-nav { display: flex; }
    main { padding: 3rem 2rem 5rem; max-width: 100%; }
    .projects-grid { grid-template-columns: 1fr; }
    .os-hero { flex-direction: column; gap: 1rem; text-align: center; }
    .os-divider { width: 60px; height: 1px; }
  }
  @media (max-width: 600px) {
    main { padding: 2rem 1.2rem 4rem; }
    .hero-name { font-size: 2.4rem; }
    .cert-grid { grid-template-columns: 1fr; }
    .hero-ctas { flex-direction: column; }
    .btn-primary, .btn-ghost { justify-content: center; }
  }

  /* ── FOOTER ── */
  .footer {
    padding: 2rem 4rem;
    border-top: 1px solid var(--border);
    font-size: 0.75rem;
    color: var(--text-3);
    font-family: var(--font-mono);
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  @media (max-width: 1024px) { .footer { padding: 1.5rem 2rem; } }
</style>
</head>
<body>

<!-- MOBILE NAV -->
<nav class="mobile-nav" id="mobileNav">
  <span class="mobile-name">Aman Srivastava</span>
  <button class="hamburger" id="hamburgerBtn" aria-label="Open menu">
    <span></span><span></span><span></span>
  </button>
</nav>

<!-- MOBILE DRAWER -->
<div class="mobile-drawer" id="mobileDrawer">
  <button class="drawer-close" id="drawerClose" aria-label="Close menu">✕</button>
  <nav class="drawer-nav">
    <a href="#about" onclick="closeDrawer()">About</a>
    <a href="#experience" onclick="closeDrawer()">Experience</a>
    <a href="#projects" onclick="closeDrawer()">Projects</a>
    <a href="#open-source" onclick="closeDrawer()">Open Source</a>
    <a href="#education" onclick="closeDrawer()">Education</a>
    <a href="#achievements" onclick="closeDrawer()">Achievements</a>
    <a href="#certifications" onclick="closeDrawer()">Certifications</a>
  </nav>
</div>

<div class="shell">

  <!-- SIDEBAR -->
  <aside class="sidebar">
    <div class="sidebar-top">
      <div class="avatar-wrap">AS</div>
      <div class="sidebar-name">Aman Srivastava</div>
      <div class="sidebar-role">Software Dev | AI/ML | Data Science</div>
      <div class="sidebar-loc">📍 New Delhi, India</div>

      <div class="nav-label">Navigation</div>
      <ul class="nav-links" id="sidebarNav">
        <li><a href="#about"><span class="dot"></span>About</a></li>
        <li><a href="#experience"><span class="dot"></span>Experience</a></li>
        <li><a href="#projects"><span class="dot"></span>Projects</a></li>
        <li><a href="#open-source"><span class="dot"></span>Open Source</a></li>
        <li><a href="#education"><span class="dot"></span>Education</a></li>
        <li><a href="#achievements"><span class="dot"></span>Achievements</a></li>
        <li><a href="#certifications"><span class="dot"></span>Certifications</a></li>
      </ul>
    </div>

    <div class="sidebar-social">
      <a href="https://github.com/aman-coder03" class="social-btn" target="_blank" rel="noopener" title="GitHub">
        <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/></svg>
      </a>
      <a href="https://linkedin.com/in/aman-srivastava03" class="social-btn" target="_blank" rel="noopener" title="LinkedIn">
        <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      </a>
      <a href="mailto:amansri345@gmail.com" class="social-btn" title="Email">
        <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
      </a>
    </div>
  </aside>

  <!-- MAIN -->
  <main>

    <!-- HERO -->
    <section id="hero">
      <div class="fade-in">
        <div class="hero-tag">
          <span class="pulse"></span>
          Available for opportunities
        </div>
        <h1 class="hero-name">Aman Srivastava<span class="cursor"></span></h1>
        <p class="hero-sub">Software Dev&nbsp;&nbsp;·&nbsp;&nbsp;AI/ML&nbsp;&nbsp;·&nbsp;&nbsp;Data Science</p>
        <p class="hero-loc">📍 New Delhi, India</p>
        <div class="hero-ctas">
          <a href="/opensource" class="btn-primary">🌐 Open Source Contributions</a>
          <a href="https://github.com/aman-coder03" class="btn-ghost" target="_blank">GitHub ↗</a>
          <a href="https://linkedin.com/in/aman-srivastava03" class="btn-ghost" target="_blank">LinkedIn ↗</a>
          <a href="mailto:amansri345@gmail.com" class="btn-ghost">Mail ↗</a>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about">
      <div class="section-eyebrow fade-in">About</div>
      <div class="about-card fade-in">
        <p>I am a final-year Computer Science undergraduate at Maharaja Surajmal Institute of Technology with interests in Artificial Intelligence, Machine Learning, Data Science, and Software Development. I enjoy building scalable, production-grade systems that combine intelligent decision-making with robust engineering.</p>
        <p>My experience spans transformer-based NLP, Retrieval-Augmented Generation (RAG), AI agents, backend development, automation platforms, and enterprise software solutions. Over the years, I have built LLM-powered applications, sentiment intelligence platforms, document retrieval systems, and workflow automation tools across diverse domains.</p>
        <p>Beyond technology, I was recommended by the Services Selection Board (SSB) for Officer Entry into the Indian Armed Forces, reflecting leadership, teamwork, and the ability to perform under pressure.</p>
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="experience">
      <div class="section-eyebrow fade-in">Experience</div>
      <h2 class="section-title fade-in">💼 Work History</h2>
      <div class="exp-list">

        <div class="exp-item fade-in">
          <div class="exp-timeline"><div class="exp-dot"></div><div class="exp-line"></div></div>
          <div class="exp-body">
            <div class="exp-card">
              <div class="exp-header">
                <div class="exp-company">System Star</div>
                <div class="exp-location">Wilmington, Delaware, United States</div>
              </div>
              <div class="exp-role">Software Development Intern</div>
              <div class="exp-date">Apr 2026 – Jun 2026</div>
              <ul class="exp-bullets">
                <li>Developed and enhanced <strong>backend services, internal tools, and automation systems</strong> supporting large-scale business operations and data-driven workflows</li>
                <li>Resolved complex production issues involving <strong>multi-threaded applications, database performance bottlenecks, concurrency failures, and system synchronization</strong>, significantly improving platform stability</li>
                <li>Designed and integrated <strong>REST APIs, workflow automation modules, and data processing pipelines</strong> to improve operational efficiency and reduce manual intervention</li>
                <li>Built centralized monitoring and reporting dashboards, aggregating data from multiple services to provide <strong>real-time system observability and operational insights</strong></li>
                <li>Performed production debugging, testing, and user acceptance validation while collaborating with engineering teams to deliver reliable and scalable software solutions</li>
              </ul>
            </div>
          </div>
        </div>

        <div class="exp-item fade-in">
          <div class="exp-timeline"><div class="exp-dot"></div><div class="exp-line"></div></div>
          <div class="exp-body">
            <div class="exp-card">
              <div class="exp-header">
                <div class="exp-company">RECONZO</div>
                <div class="exp-location">Gurugram, Haryana, India</div>
              </div>
              <div class="exp-role">Competitive Intelligence Intern</div>
              <div class="exp-date">Dec 2025 – Feb 2026</div>
              <ul class="exp-bullets">
                <li>Built a data-driven competitive intelligence framework to analyze <strong>market pricing, promotional strategies, inventory trends, and competitor positioning</strong> across leading retail and quick-commerce platforms</li>
                <li>Processed large-scale market datasets and improved analytical throughput by <strong>~7×</strong>, enabling timely identification of emerging business opportunities and competitive risks</li>
                <li>Performed pricing and inventory analytics to uncover <strong>discount volatility, stock movement patterns, and regional demand variations</strong> across multiple markets</li>
                <li>Developed ETL workflows and structured reporting systems that generated <strong>pricing intelligence, margin insights, and strategic business recommendations</strong></li>
                <li>Delivered actionable insights through automated dashboards and analytics pipelines, supporting <strong>data-driven decision-making and competitive strategy formulation</strong></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="exp-item fade-in">
          <div class="exp-timeline"><div class="exp-dot"></div><div class="exp-line"></div></div>
          <div class="exp-body">
            <div class="exp-card">
              <div class="exp-header">
                <div class="exp-company">Indian Institute of Technology Delhi</div>
                <div class="exp-location">New Delhi, India</div>
              </div>
              <div class="exp-role">AI/ML Intern</div>
              <div class="exp-date">Jun 2025 – Jul 2025</div>
              <ul class="exp-bullets">
                <li>Architected and deployed <strong>LibSenti</strong>, a transformer-based sentiment intelligence platform analyzing <strong>10,000+ institutional reviews</strong> for large-scale opinion mining and sentiment analytics</li>
                <li>Fine-tuned a <strong>RoBERTa model using PyTorch and Hugging Face Transformers</strong>, achieving <strong>95%+ classification accuracy</strong> through advanced preprocessing, class balancing, and label smoothing techniques</li>
                <li>Designed scalable NLP pipelines for data cleaning, tokenization, augmentation, model training, evaluation, and inference, improving model robustness and generalization</li>
                <li>Built and deployed a <strong>real-time sentiment analysis application</strong> using Streamlit and Hugging Face Hub, enabling interactive inference, confidence visualization, and explainable predictions</li>
                <li>Developed comprehensive evaluation workflows leveraging precision, recall, F1-score, confusion matrices, and error analysis to optimize model performance across sentiment classes</li>
                <li>Automated validation and publishing workflows for <strong>15,000+ Drupal CMS records</strong>, reducing manual effort by <strong>60%</strong> and improving operational efficiency by <strong>3×</strong></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="exp-item fade-in">
          <div class="exp-timeline"><div class="exp-dot"></div><div class="exp-line"></div></div>
          <div class="exp-body">
            <div class="exp-card">
              <div class="exp-header">
                <div class="exp-company">CEERAS</div>
                <div class="exp-location">Cuddapah, Andhra Pradesh, India</div>
              </div>
              <div class="exp-role">Software Developer Intern</div>
              <div class="exp-date">Feb 2025 – Jun 2025</div>
              <ul class="exp-bullets">
                <li>Engineered a gamified coding platform used by <strong>1,000+ kids</strong></li>
                <li>Improved backend performance by <strong>15%</strong> and user engagement by <strong>30%</strong></li>
              </ul>
            </div>
          </div>
        </div>

        <div class="exp-item fade-in">
          <div class="exp-timeline"><div class="exp-dot"></div><div class="exp-line"></div></div>
          <div class="exp-body">
            <div class="exp-card">
              <div class="exp-header">
                <div class="exp-company">U-Knighted Chess Society</div>
                <div class="exp-location">New Delhi, India</div>
              </div>
              <div class="exp-role">Founder &amp; President</div>
              <div class="exp-date">Jan 2025 – Present</div>
              <ul class="exp-bullets">
                <li>Founded and scaled the college chess society to <strong>100+ active members</strong>, building one of the largest student-led strategic gaming communities on campus</li>
                <li>Led a <strong>15-member core team</strong>, overseeing event planning, operations, partnerships, community engagement, and organizational growth</li>
                <li>Organized inter-college tournaments, competitive events, and strategy workshops, driving sustained member participation and skill development</li>
                <li>Secured sponsorship from <strong>Smaaash</strong> and established external partnerships, enabling the successful execution of multiple sponsored events</li>
                <li>Managed budgeting, stakeholder coordination, and event logistics while fostering a collaborative and high-performance community culture</li>
              </ul>
            </div>
          </div>
        </div>

      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects">
      <div class="section-eyebrow fade-in">Projects</div>
      <h2 class="section-title fade-in">🧠 Projects</h2>
      <div class="projects-grid">

        <div class="proj-card fade-in">
          <div class="proj-icon">🗄️</div>
          <div class="proj-name">DIRS – Document Intelligence &amp; Retrieval System</div>
          <ul class="proj-bullets">
            <li>Built an enterprise-grade RAG platform converting unstructured PDFs into a searchable semantic knowledge base using FAISS, ChromaDB, Milvus, and Qdrant</li>
            <li>Implemented hybrid retrieval combining vector similarity search with BM25 score fusion, improving retrieval accuracy across diverse document collections</li>
            <li>Integrated local LLM inference using LLaMA, Qwen, and Gemma models for secure and privacy-preserving document question answering</li>
            <li>Designed role-based access control and modular ingestion pipelines for secure enterprise document intelligence workflows</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">🤖</div>
          <div class="proj-name">ShadowVerse – Autonomous AI Agent</div>
          <ul class="proj-bullets">
            <li>Developed an AI-powered autonomous agent capable of identifying relevant jobs, selecting optimized resumes, generating personalized cover letters, and automating applications</li>
            <li>Built browser automation workflows for job discovery, form completion, recruiter outreach, and application tracking</li>
            <li>Integrated resume intelligence, job matching, and LLM-driven personalization into a unified application ecosystem</li>
            <li>Designed scalable architecture supporting autonomous job search across multiple recruitment platforms</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">🔬</div>
          <div class="proj-name">Wafer Shield AI – Edge AI Semiconductor Defect Classification</div>
          <ul class="proj-bullets">
            <li>Deployed an edge-optimized semiconductor defect classification system using EfficientNetLite0 achieving <strong>90.34% accuracy</strong></li>
            <li>Built a lightweight 6.76 MB FP16 ONNX model achieving <strong>8.55 ms CPU latency</strong> and <strong>116.9 images/sec throughput</strong></li>
            <li>Engineered optimized preprocessing and inference pipelines for deployment in low-resource industrial environments</li>
            <li>Reduced computational requirements while maintaining production-grade defect detection performance</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">💬</div>
          <div class="proj-name">LibSenti – Transformer-Based Sentiment Intelligence Platform</div>
          <ul class="proj-bullets">
            <li>Built an end-to-end sentiment intelligence platform analyzing <strong>10,000+ IIT and NIT library reviews</strong> using transformer-based NLP</li>
            <li>Fine-tuned a RoBERTa model achieving <strong>95%+ classification accuracy</strong> through advanced preprocessing, class balancing, and label smoothing</li>
            <li>Developed a real-time Streamlit application enabling interactive predictions, confidence visualization, and institutional analytics</li>
            <li>Designed scalable NLP pipelines supporting large-scale sentiment monitoring and reporting</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">🏢</div>
          <div class="proj-name">CLAMANS – Enterprise Leave Management System</div>
          <ul class="proj-bullets">
            <li>Designed and developed a role-based institutional leave management platform for IIT Delhi</li>
            <li>Implemented PostgreSQL-based leave computation logic supporting holiday policies, approval workflows, and leave balance tracking</li>
            <li>Built OTP authentication, email notifications, and automated workflow management using SMTP services</li>
            <li>Created secure administrative and employee portals with end-to-end workflow automation</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">⚖️</div>
          <div class="proj-name">FinRisk – Financial Compliance Intelligence System</div>
          <ul class="proj-bullets">
            <li>Built a multi-source financial intelligence platform monitoring AML, sanctions, fraud, regulatory, and compliance-related developments</li>
            <li>Developed a weighted risk scoring engine across 25+ compliance indicators for automated threat prioritization</li>
            <li>Designed KPI dashboards and automated reporting systems supporting risk assessment and investigation workflows</li>
            <li>Implemented data aggregation pipelines for large-scale compliance intelligence generation</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">☀️</div>
          <div class="proj-name">SolarAI Assistant</div>
          <ul class="proj-bullets">
            <li>Built an AI-powered rooftop solar advisory platform integrating subsidy calculations, ROI estimation, and energy generation forecasting</li>
            <li>Implemented PM Surya Ghar policy logic and financial simulations for personalized investment recommendations</li>
            <li>Generated location-aware solar installation insights based on energy consumption patterns and infrastructure constraints</li>
            <li>Automated cost-benefit analysis to support informed renewable energy adoption decisions</li>
          </ul>
        </div>

        <div class="proj-card fade-in">
          <div class="proj-icon">✉️</div>
          <div class="proj-name">SmartMailer – AI Email Automation</div>
          <ul class="proj-bullets">
            <li>Developed an NLP-powered email generation and automation platform for professional communication workflows</li>
            <li>Automated email drafting, personalization, and delivery processes, reducing drafting time by <strong>75%</strong></li>
            <li>Integrated intelligent content generation and workflow automation, eliminating <strong>65%</strong> of manual effort</li>
            <li>Built scalable modules for bulk communication and personalized outreach campaigns</li>
          </ul>
        </div>

      </div>
    </section>

    <!-- OPEN SOURCE -->
    <section id="open-source">
      <div class="section-eyebrow fade-in">Open Source</div>
      <h2 class="section-title fade-in">🌐 Contributions</h2>
      <div class="os-hero fade-in">
        <div class="os-stat">
          <div class="os-number">24+</div>
          <div class="os-label">Merged PRs</div>
        </div>
        <div class="os-divider"></div>
        <div class="os-desc">
          Active open-source contributor with <strong>24+ merged pull requests across globally used projects</strong>, contributing to machine learning, scientific computing, visualization, and developer tooling ecosystems.
          <div class="os-ecosystems">
            <span class="eco-tag">Machine Learning</span>
            <span class="eco-tag">Scientific Computing</span>
            <span class="eco-tag">Data Visualization</span>
            <span class="eco-tag">Developer Tooling</span>
          </div>
          <a href="/opensource" class="os-link">View all contributions →</a>
        </div>
      </div>
    </section>

    <!-- EDUCATION -->
    <section id="education">
      <div class="section-eyebrow fade-in">Education</div>
      <h2 class="section-title fade-in">🎓 Education</h2>
      <div class="edu-grid">
        <div class="edu-card fade-in">
          <div class="edu-icon">🏛️</div>
          <div>
            <div class="edu-inst">Maharaja Surajmal Institute of Technology (GGSIPU)</div>
            <div class="edu-degree">B.Tech in Computer Science Engineering</div>
            <div class="edu-meta">2023 – 2027</div>
          </div>
        </div>
        <div class="edu-card fade-in">
          <div class="edu-icon">🏫</div>
          <div>
            <div class="edu-inst">DAV Vasant Kunj</div>
            <div class="edu-degree">Grade 12 (PCM) · School Topper in Computer Science</div>
            <div class="edu-meta">2022 – 2023</div>
          </div>
        </div>
      </div>
    </section>

    <!-- ACHIEVEMENTS -->
    <section id="achievements">
      <div class="section-eyebrow fade-in">Recognition</div>
      <h2 class="section-title fade-in">🏆 Achievements</h2>
      <div class="ach-grid">
        <div class="ach-card fade-in">
          <div class="ach-badge">🌏</div>
          <div>
            <div class="ach-title">Globally Selected – Hacker House 2024, Bangkok</div>
          </div>
        </div>
        <div class="ach-card fade-in">
          <div class="ach-badge">🥇</div>
          <div>
            <div class="ach-title">Top 50 / 500+ teams – Hack for Impact 2025, IIIT Delhi</div>
          </div>
        </div>
      </div>
    </section>

    <!-- CERTIFICATIONS -->
    <section id="certifications">
      <div class="section-eyebrow fade-in">Credentials</div>
      <h2 class="section-title fade-in">📜 Certifications</h2>
      <div class="cert-grid">
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">80+ Google Cloud Skill Badges</div>
            <div class="cert-issuer">Cloud Infrastructure, AI/ML, Data Engineering, Generative AI</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Global Markets Sales &amp; Trading Analyst</div>
            <div class="cert-issuer">Bank of America</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Artificial Intelligence Fundamentals</div>
            <div class="cert-issuer">IBM</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Cloud Computing Foundations</div>
            <div class="cert-issuer">Google Cloud</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Data Analytics Job Simulation</div>
            <div class="cert-issuer">Quantium</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Data Analytics Job Simulation</div>
            <div class="cert-issuer">Deloitte</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">GenAI Job Simulation</div>
            <div class="cert-issuer">Boston Consulting Group</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">SQL Advanced</div>
            <div class="cert-issuer">HackerRank</div>
          </div>
        </div>
        <div class="cert-card fade-in">
          <div class="cert-dot"></div>
          <div>
            <div class="cert-name">Data Quality &amp; Consistency with ODE</div>
            <div class="cert-issuer">Open Knowledge Brasil</div>
          </div>
        </div>
      </div>
    </section>

  </main>
</div>

<footer class="footer">
  <span>Aman Srivastava · amansri345@gmail.com</span>
  <span>New Delhi, India</span>
</footer>

<script>
  // Intersection Observer for fade-in
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        // stagger children if it's a grid
        const children = entry.target.querySelectorAll('.fade-in');
        children.forEach((child, i) => {
          setTimeout(() => child.classList.add('visible'), i * 60);
        });
      }
    });
  }, { threshold: 0.08 });

  document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

  // Active nav link on scroll
  const sections = document.querySelectorAll('section[id]');
  const navLinks = document.querySelectorAll('#sidebarNav a');

  const navObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        navLinks.forEach(link => {
          link.classList.remove('active');
          if (link.getAttribute('href') === '#' + entry.target.id) {
            link.classList.add('active');
          }
        });
      }
    });
  }, { rootMargin: '-30% 0px -60% 0px' });

  sections.forEach(s => navObserver.observe(s));

  // Mobile drawer
  const hamburgerBtn = document.getElementById('hamburgerBtn');
  const drawer = document.getElementById('mobileDrawer');
  const drawerClose = document.getElementById('drawerClose');

  hamburgerBtn.addEventListener('click', () => drawer.classList.add('open'));
  drawerClose.addEventListener('click', closeDrawer);
  drawer.addEventListener('click', e => { if (e.target === drawer) closeDrawer(); });
  function closeDrawer() { drawer.classList.remove('open'); }

  // Respect reduced motion
  if (window.matchMedia('(prefers-reduced-motion: reduce)').matches) {
    document.querySelectorAll('.fade-in').forEach(el => {
      el.style.opacity = '1';
      el.style.transform = 'none';
    });
  }
</script>
</body>
</html>
