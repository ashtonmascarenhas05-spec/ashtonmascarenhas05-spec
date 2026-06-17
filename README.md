<img src="IMG_20260617_180149.png.jpg" alt="Ashton Avatar" width="250" style="border-radius: 15px; box-shadow: 0px 4px 10px rgba(0,255,0,0.2);" />

<style>
  @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600&family=Inter:wght@400;500&display=swap');

  .pr {
    font-family: 'Inter', sans-serif;
    background: #0d0d14;
    border-radius: 16px;
    padding: 0 0 4px;
    overflow: hidden;
    color: #e2e0f0;
  }

  .hero {
    background: linear-gradient(135deg, #12102a 0%, #160e28 60%, #0e1520 100%);
    padding: 28px 28px 24px;
    position: relative;
    border-bottom: 1px solid #2a1f4a;
  }

  .hero-accent-bar {
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: linear-gradient(90deg, #7c3aed, #ec4899, #f59e0b);
  }

  .hero-inner {
    display: grid;
    grid-template-columns: 100px 1fr;
    gap: 20px;
    align-items: center;
  }

  .avatar {
    width: 88px;
    height: 88px;
    border-radius: 14px;
    background: linear-gradient(135deg, #7c3aed, #ec4899);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'JetBrains Mono', monospace;
    font-size: 26px;
    font-weight: 600;
    color: #fff;
    position: relative;
  }

  .avatar::after {
    content: '';
    position: absolute;
    inset: -2px;
    border-radius: 15px;
    background: linear-gradient(135deg, #7c3aed, #ec4899, #f59e0b);
    z-index: -1;
  }

  .hero-name {
    font-family: 'JetBrains Mono', monospace;
    font-size: 19px;
    font-weight: 600;
    color: #f0eeff;
    margin: 0 0 3px;
  }

  .hero-handle {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    color: #a78bfa;
    margin: 0 0 8px;
  }

  .hero-bio {
    font-size: 13px;
    color: #9ca0c4;
    margin: 0 0 10px;
    line-height: 1.5;
  }

  .hero-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .pill {
    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
    padding: 3px 9px;
    border-radius: 20px;
    font-weight: 600;
    letter-spacing: 0.03em;
  }

  .pill-purple { background: #2d1b69; color: #c4b5fd; border: 1px solid #4c1d95; }
  .pill-pink   { background: #3b0a2a; color: #f9a8d4; border: 1px solid #831843; }
  .pill-amber  { background: #2a1a00; color: #fcd34d; border: 1px solid #78350f; }
  .pill-teal   { background: #042f2e; color: #5eead4; border: 1px solid #134e4a; }

  .body {
    padding: 16px 20px;
    display: flex;
    flex-direction: column;
    gap: 14px;
  }

  .row2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
  }

  .card {
    background: #12101f;
    border: 1px solid #1e1a35;
    border-radius: 12px;
    padding: 16px 18px;
  }

  .sec-label {
    font-family: 'JetBrains Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin: 0 0 12px;
    display: flex;
    align-items: center;
    gap: 7px;
  }

  .dot-purple { width:6px;height:6px;border-radius:50%;background:#7c3aed;flex-shrink:0; }
  .dot-pink   { width:6px;height:6px;border-radius:50%;background:#ec4899;flex-shrink:0; }
  .dot-amber  { width:6px;height:6px;border-radius:50%;background:#f59e0b;flex-shrink:0; }
  .dot-teal   { width:6px;height:6px;border-radius:50%;background:#14b8a6;flex-shrink:0; }

  .label-purple { color: #a78bfa; }
  .label-pink   { color: #f472b6; }
  .label-amber  { color: #fbbf24; }
  .label-teal   { color: #2dd4bf; }

  .skill-row {
    display: flex;
    align-items: center;
    gap: 8px;
    margin-bottom: 9px;
  }

  .skill-row:last-child { margin-bottom: 0; }

  .skill-row i {
    font-size: 14px;
    width: 16px;
    text-align: center;
    flex-shrink: 0;
  }

  .skill-name {
    font-size: 12px;
    color: #ccc8e8;
    min-width: 82px;
  }

  .bar-bg {
    flex: 1;
    height: 3px;
    background: #1e1a35;
    border-radius: 2px;
    overflow: hidden;
  }

  .bar-fill {
    height: 100%;
    border-radius: 2px;
  }

  .bar-purple { background: linear-gradient(90deg, #7c3aed, #a78bfa); }
  .bar-pink   { background: linear-gradient(90deg, #ec4899, #f9a8d4); }
  .bar-amber  { background: linear-gradient(90deg, #f59e0b, #fcd34d); }
  .bar-teal   { background: linear-gradient(90deg, #14b8a6, #5eead4); }

  .focus-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 8px;
  }

  .focus-chip {
    display: flex;
    align-items: center;
    gap: 8px;
    background: #0f0d1c;
    border: 1px solid #1e1a35;
    border-radius: 8px;
    padding: 9px 12px;
    font-size: 12px;
    color: #ccc8e8;
  }

  .focus-chip i {
    font-size: 15px;
    flex-shrink: 0;
  }

  .hobby-row {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 8px 0;
    border-bottom: 1px solid #1a1730;
  }

  .hobby-row:last-child { border-bottom: none; padding-bottom: 0; }
  .hobby-row:first-child { padding-top: 0; }

  .hobby-icon-box {
    width: 34px;
    height: 34px;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
  }

  .hib-pink   { background: #3b0a2a; border: 1px solid #9d174d; }
  .hib-amber  { background: #2a1a00; border: 1px solid #92400e; }

  .hobby-icon-box i { font-size: 16px; }
  .ic-pink { color: #f472b6; }
  .ic-amber { color: #fbbf24; }

  .hobby-info { display: flex; flex-direction: column; gap: 2px; }
  .hobby-title { font-size: 13px; font-weight: 500; color: #e2e0f0; margin: 0; }
  .hobby-sub   { font-size: 11px; color: #6b6891; margin: 0; }

  .connect-card {
    background: linear-gradient(135deg, #12102a, #0e1520);
    border: 1px solid #1e1a35;
    border-radius: 12px;
    padding: 16px 18px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
  }

  .connect-left { display: flex; flex-direction: column; gap: 3px; }
  .connect-name { font-size: 13px; font-weight: 500; color: #e2e0f0; margin: 0; }
  .connect-sub  { font-size: 11px; color: #6b6891; margin: 0; }

  .linkedin-btn {
    display: flex;
    align-items: center;
    gap: 7px;
    padding: 9px 18px;
    border-radius: 8px;
    border: 1px solid #1d4ed8;
    background: #172554;
    color: #93c5fd;
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    text-decoration: none;
    transition: background 0.15s;
    flex-shrink: 0;
    cursor: pointer;
  }

  .linkedin-btn:hover { background: #1e3a8a; }
  .linkedin-btn i { font-size: 15px; }

  .footer-bar {
    padding: 12px 20px 14px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-top: 1px solid #1a1730;
  }

  .footer-bar span {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: #3d3860;
  }

  .footer-bar .sym { color: #7c3aed; }

  .cursor {
    display: inline-block;
    width: 7px;
    height: 12px;
    background: #7c3aed;
    border-radius: 1px;
    animation: blink 1.1s step-end infinite;
    vertical-align: -2px;
  }

  @keyframes blink { 50% { opacity: 0; } }
</style>

<div class="pr">
  <div class="hero">
    <div class="hero-accent-bar"></div>
    <div class="hero-inner">
      <div class="avatar">AA</div>
      <div>
        <p class="hero-name">Ashton Alex Mascarenhas</p>
        <p class="hero-handle">@ashton0803</p>
        <p class="hero-bio">SY AIML Student — building at the intersection of ML, MLOps & Agentic AI</p>
        <div class="hero-pills">
          <span class="pill pill-purple">ML</span>
          <span class="pill pill-pink">MLOps</span>
          <span class="pill pill-amber">AI Agents</span>
          <span class="pill pill-teal">Python</span>
        </div>
      </div>
    </div>
  </div>

  <div class="body">
    <div class="card">
      <div class="sec-label"><div class="dot-teal"></div><span class="label-teal">Current focus</span></div>
      <div class="focus-grid">
        <div class="focus-chip"><i class="ti ti-cpu" style="color:#2dd4bf" aria-hidden="true"></i>Machine learning</div>
        <div class="focus-chip"><i class="ti ti-route" style="color:#a78bfa" aria-hidden="true"></i>MLOps pipelines</div>
        <div class="focus-chip"><i class="ti ti-robot" style="color:#f472b6" aria-hidden="true"></i>Agentic AI</div>
        <div class="focus-chip"><i class="ti ti-chart-dots" style="color:#fbbf24" aria-hidden="true"></i>Data analysis</div>
      </div>
    </div>

    <div class="row2">
      <div class="card">
        <div class="sec-label"><div class="dot-purple"></div><span class="label-purple">Technical skills</span></div>
        <div class="skill-row">
          <i class="ti ti-brand-python" style="color:#a78bfa" aria-hidden="true"></i>
          <span class="skill-name">Python</span>
          <div class="bar-bg"><div class="bar-fill bar-purple" style="width:85%"></div></div>
        </div>
        <div class="skill-row">
          <i class="ti ti-chart-bar" style="color:#f472b6" aria-hidden="true"></i>
          <span class="skill-name">Data analysis</span>
          <div class="bar-bg"><div class="bar-fill bar-pink" style="width:72%"></div></div>
        </div>
        <div class="skill-row">
          <i class="ti ti-brain" style="color:#fbbf24" aria-hidden="true"></i>
          <span class="skill-name">ML models</span>
          <div class="bar-bg"><div class="bar-fill bar-amber" style="width:60%"></div></div>
        </div>
        <div class="skill-row">
          <i class="ti ti-settings-automation" style="color:#2dd4bf" aria-hidden="true"></i>
          <span class="skill-name">MLOps</span>
          <div class="bar-bg"><div class="bar-fill bar-teal" style="width:45%"></div></div>
        </div>
      </div>

      <div class="card">
        <div class="sec-label"><div class="dot-pink"></div><span class="label-pink">Beyond the code</span></div>
        <div class="hobby-row">
          <div class="hobby-icon-box hib-pink">
            <i class="ti ti-piano ic-pink" aria-hidden="true"></i>
          </div>
          <div class="hobby-info">
            <p class="hobby-title">Keyboardist</p>
            <p class="hobby-sub">Chord theory & composition</p>
          </div>
        </div>
        <div class="hobby-row">
          <div class="hobby-icon-box hib-amber">
            <i class="ti ti-music ic-amber" aria-hidden="true"></i>
          </div>
          <div class="hobby-info">
            <p class="hobby-title">Music production</p>
            <p class="hobby-sub">Digital audio & sound design</p>
          </div>
        </div>
      </div>
    </div>

    <div class="connect-card">
      <div class="connect-left">
        <div class="sec-label" style="margin:0 0 4px"><div class="dot-teal"></div><span class="label-teal">Connect</span></div>
        <p class="connect-name">Ashton Alex Mascarenhas</p>
        <p class="connect-sub">linkedin.com/in/ashton0803</p>
      </div>
      <a href="https://www.linkedin.com/in/ashton0803/" class="linkedin-btn" target="_blank">
        <i class="ti ti-brand-linkedin" aria-hidden="true"></i>
        View profile
      </a>
    </div>
  </div>

  <div class="footer-bar">
    <span class="sym">~/ashton0803 $</span>
    <span>git push origin main</span>
    <span class="cursor"></span>
  </div>
</div>


