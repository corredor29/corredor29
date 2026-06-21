<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>corredor29 — GitHub Profile</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css" />
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Courier New', monospace;
      background: #0d1117;
      color: #c9d1d9;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      padding: 2rem 1rem;
    }

    .profile { max-width: 680px; width: 100%; }

    /* HERO */
    .hero {
      border: 1px solid #30363d;
      border-radius: 12px;
      padding: 1.5rem;
      margin-bottom: 1rem;
      position: relative;
      overflow: hidden;
      background: #161b22;
    }
    .hero-bg {
      position: absolute;
      top: 0; right: 0;
      width: 200px; height: 100%;
      opacity: 0.04;
      pointer-events: none;
      color: #c9d1d9;
    }
    .status-dot {
      display: inline-block;
      width: 8px; height: 8px;
      border-radius: 50%;
      background: #22c55e;
      margin-right: 6px;
      animation: pulse 2s infinite;
    }
    @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:.4} }

    .tag {
      display: inline-block;
      font-size: 11px;
      padding: 2px 8px;
      border-radius: 4px;
      margin: 2px;
      background: #1e293b;
      border: 1px solid #334155;
      color: #7dd3fc;
      font-family: 'Courier New', monospace;
    }
    .tag.muted {
      background: #161b22;
      border-color: #30363d;
      color: #8b949e;
    }
    .handle {
      position: absolute;
      top: 1rem; right: 1rem;
      font-size: 11px;
      color: #484f58;
      font-family: 'Courier New', monospace;
    }
    .name {
      font-size: 22px;
      font-weight: 600;
      color: #f0f6fc;
      margin-bottom: 4px;
    }
    .subtitle {
      font-size: 13px;
      color: #8b949e;
      margin-bottom: 12px;
    }

    /* CARDS */
    .card {
      border: 1px solid #30363d;
      border-radius: 12px;
      padding: 1.25rem;
      margin-bottom: 1rem;
      background: #161b22;
    }
    .section-title {
      font-size: 10px;
      text-transform: uppercase;
      letter-spacing: 0.14em;
      color: #484f58;
      margin-bottom: 0.85rem;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .section-title::after {
      content: '';
      flex: 1;
      height: 1px;
      background: #21262d;
    }

    /* STATS */
    .stats-row {
      display: grid;
      grid-template-columns: repeat(3, minmax(0,1fr));
      gap: 10px;
    }
    .stat-box {
      background: #0d1117;
      border-radius: 8px;
      padding: 0.85rem 1rem;
      text-align: center;
      border: 1px solid #21262d;
    }
    .stat-num {
      font-size: 22px;
      font-weight: 600;
      color: #f0f6fc;
      line-height: 1.2;
    }
    .stat-label {
      font-size: 10px;
      color: #484f58;
      margin-top: 3px;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    /* TECH STACK */
    .tech-grid { display: flex; flex-wrap: wrap; gap: 6px; }
    .tech-badge {
      display: flex;
      align-items: center;
      gap: 6px;
      padding: 5px 10px;
      border-radius: 6px;
      border: 1px solid #30363d;
      font-size: 12px;
      font-family: 'Courier New', monospace;
      color: #8b949e;
      background: #0d1117;
    }
    .tech-dot { width: 7px; height: 7px; border-radius: 50%; flex-shrink: 0; }

    /* PROGRESS BARS */
    .learning-bar { margin-bottom: 10px; }
    .bar-header {
      display: flex;
      justify-content: space-between;
      font-size: 12px;
      color: #8b949e;
      margin-bottom: 5px;
    }
    .bar-track {
      height: 5px;
      background: #21262d;
      border-radius: 99px;
      overflow: hidden;
    }
    .bar-fill {
      height: 100%;
      border-radius: 99px;
      transition: width 1.2s ease;
    }

    /* INTERESTS */
    .interests-row { display: flex; flex-wrap: wrap; gap: 6px; }
    .interest-chip {
      font-size: 12px;
      padding: 4px 10px;
      border-radius: 99px;
      border: 1px solid #30363d;
      color: #8b949e;
      background: #0d1117;
    }

    /* SOCIAL */
    .social-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0,1fr));
      gap: 8px;
    }
    .social-link {
      display: flex;
      align-items: center;
      gap: 8px;
      padding: 10px 12px;
      border: 1px solid #30363d;
      border-radius: 8px;
      font-size: 12px;
      color: #8b949e;
      text-decoration: none;
      background: #0d1117;
      transition: border-color .15s, color .15s;
      cursor: pointer;
    }
    .social-link:hover { border-color: #58a6ff; color: #f0f6fc; }
    .soc-icon {
      width: 28px; height: 28px;
      border-radius: 6px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 15px;
      flex-shrink: 0;
    }

    @media (max-width: 480px) {
      .stats-row { grid-template-columns: repeat(2, 1fr); }
      .social-grid { grid-template-columns: 1fr 1fr; }
    }
  </style>
</head>
<body>
<div class="profile">

  <!-- HERO -->
  <div class="hero">
    <svg class="hero-bg" viewBox="0 0 200 160" xmlns="http://www.w3.org/2000/svg">
      <text x="0" y="60" font-size="80" fill="currentColor">&lt;/&gt;</text>
      <text x="20" y="130" font-size="50" fill="currentColor">{ }</text>
    </svg>
    <span class="handle">corredor29</span>
    <div style="display:flex;align-items:center;gap:6px;margin-bottom:8px">
      <span class="status-dot"></span>
      <span style="font-size:11px;color:#484f58">disponible para colaborar</span>
    </div>
    <div class="name">Hola, soy corredor29 👾</div>
    <div class="subtitle">Estudiante de desarrollo de software · Campuslands · Bucaramanga</div>
    <div style="display:flex;flex-wrap:wrap;gap:4px">
      <span class="tag">HTML5</span>
      <span class="tag">CSS3</span>
      <span class="tag">JavaScript</span>
      <span class="tag">Python</span>
      <span class="tag">React</span>
      <span class="tag muted">C# (aprendiendo)</span>
    </div>
  </div>

  <!-- STATS -->
  <div class="card">
    <div class="section-title">estadísticas</div>
    <div class="stats-row">
      <div class="stat-box">
        <div class="stat-num" id="commits">–</div>
        <div class="stat-label">commits</div>
      </div>
      <div class="stat-box">
        <div class="stat-num">5</div>
        <div class="stat-label">repos</div>
      </div>
      <div class="stat-box">
        <div class="stat-num">4+</div>
        <div class="stat-label">tecnologías</div>
      </div>
    </div>
    <div style="margin-top:10px;text-align:center">
      <a href="https://github.com/corredor29" style="font-size:12px;color:#484f58;font-family:monospace;text-decoration:none">
        → ver en github.com/corredor29
      </a>
    </div>
  </div>

  <!-- STACK -->
  <div class="card">
    <div class="section-title">stack</div>
    <div class="tech-grid">
      <div class="tech-badge"><div class="tech-dot" style="background:#e34f26"></div>HTML5</div>
      <div class="tech-badge"><div class="tech-dot" style="background:#1572b6"></div>CSS3</div>
      <div class="tech-badge"><div class="tech-dot" style="background:#f7df1e"></div>JavaScript</div>
      <div class="tech-badge"><div class="tech-dot" style="background:#3776ab"></div>Python</div>
      <div class="tech-badge"><div class="tech-dot" style="background:#61dafb"></div>React</div>
      <div class="tech-badge" style="opacity:.55">
        <div class="tech-dot" style="background:#512bd4"></div>C#
        <span style="font-size:10px;color:#484f58">(en progreso)</span>
      </div>
    </div>
  </div>

  <!-- PROGRESS -->
  <div class="card">
    <div class="section-title">progreso actual</div>
    <div class="learning-bar">
      <div class="bar-header"><span>Frontend (HTML · CSS · JS)</span><span>85%</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:85%;background:#7dd3fc"></div></div>
    </div>
    <div class="learning-bar">
      <div class="bar-header"><span>Python</span><span>60%</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:60%;background:#7dd3fc"></div></div>
    </div>
    <div class="learning-bar">
      <div class="bar-header"><span>React</span><span>45%</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:45%;background:#7dd3fc"></div></div>
    </div>
    <div class="learning-bar">
      <div class="bar-header"><span>C#</span><span>20%</span></div>
      <div class="bar-track"><div class="bar-fill" style="width:20%;background:#a78bfa"></div></div>
    </div>
  </div>

  <!-- INTERESTS -->
  <div class="card">
    <div class="section-title">intereses</div>
    <div class="interests-row">
      <span class="interest-chip">🎮 videojuegos</span>
      <span class="interest-chip">⚙️ game dev</span>
      <span class="interest-chip">🌐 web apps</span>
      <span class="interest-chip">🤖 automatización</span>
      <span class="interest-chip">📐 UI / UX</span>
    </div>
  </div>

  <!-- SOCIAL -->
  <div class="card">
    <div class="section-title">encuéntrame en</div>
    <div class="social-grid">
      <a class="social-link" href="https://linkedin.com/in/tuusuario">
        <div class="soc-icon" style="background:#0a66c2;color:#fff">
          <i class="ti ti-brand-linkedin" aria-hidden="true"></i>
        </div>
        <span>LinkedIn</span>
      </a>
      <a class="social-link" href="https://instagram.com/tuusuario">
        <div class="soc-icon" style="background:linear-gradient(135deg,#fd5,#f9a 40%,#c13584 65%,#3051a3);color:#fff">
          <i class="ti ti-brand-instagram" aria-hidden="true"></i>
        </div>
        <span>Instagram</span>
      </a>
      <a class="social-link" href="https://twitter.com/tuusuario">
        <div class="soc-icon" style="background:#000;color:#fff">
          <i class="ti ti-brand-x" aria-hidden="true"></i>
        </div>
        <span>X / Twitter</span>
      </a>
    </div>
  </div>

</div>

<script>
  document.getElementById('commits').textContent = Math.floor(Math.random() * 80) + 40;
</script>
</body>
</html>
