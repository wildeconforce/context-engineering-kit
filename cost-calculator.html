<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Context Engineering — Cost Calculator</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;1,9..144,400&family=Instrument+Sans:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #F4EFE4;
    --bg-panel: #FBF7ED;
    --bg-card: #FFFFFF;
    --ink: #1C1917;
    --ink-soft: #57534E;
    --ink-mute: #A8A29E;
    --line: #E7E1D2;
    --line-soft: #EFEAE0;
    --accent: #B45309;
    --accent-warm: #D97706;
    --accent-dark: #7C2D12;
    --bad: #B91C1C;
    --ok: #047857;
    --grad-hero: linear-gradient(95deg, #D97706 0%, #B45309 30%, #9A3412 55%, #047857 100%);
    --grad-card: linear-gradient(160deg, #FEF3C7 0%, #FED7AA 40%, #FDBA74 100%);
    --grad-savings: linear-gradient(135deg, #EAB308 0%, #D97706 40%, #047857 100%);
    --shadow-sm: 0 1px 2px rgba(28, 25, 23, 0.04);
    --shadow-md: 0 4px 20px -4px rgba(28, 25, 23, 0.08), 0 2px 6px -2px rgba(28, 25, 23, 0.04);
    --shadow-lg: 0 20px 60px -20px rgba(124, 45, 18, 0.18), 0 8px 24px -8px rgba(28, 25, 23, 0.1);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  html, body {
    background: var(--bg);
    color: var(--ink);
    font-family: 'Instrument Sans', system-ui, sans-serif;
    font-size: 16px;
    line-height: 1.55;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    overflow-x: hidden;
  }

  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image:
      radial-gradient(1200px 600px at 85% -10%, rgba(234, 179, 8, 0.08), transparent 60%),
      radial-gradient(900px 500px at -10% 110%, rgba(4, 120, 87, 0.06), transparent 60%);
    pointer-events: none;
    z-index: 0;
  }

  body::after {
    content: '';
    position: fixed;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='2' stitchTiles='stitch'/%3E%3CfeColorMatrix values='0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.12 0'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
    opacity: 0.35;
    pointer-events: none;
    z-index: 0;
    mix-blend-mode: multiply;
  }

  .wrap {
    position: relative;
    z-index: 1;
    max-width: 1240px;
    margin: 0 auto;
    padding: 48px 32px 80px;
  }

  /* ─── Header ──────────────────────────────────────────── */
  header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding-bottom: 20px;
    border-bottom: 1px solid var(--line);
    margin-bottom: 56px;
    gap: 24px;
    flex-wrap: wrap;
  }
  .brand {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    font-weight: 500;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--ink-soft);
  }
  .brand::before {
    content: '◆';
    color: var(--accent);
    margin-right: 8px;
    font-size: 10px;
  }
  .header-meta {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.1em;
    color: var(--ink-mute);
    text-transform: uppercase;
  }

  /* ─── Hero ────────────────────────────────────────────── */
  .hero {
    text-align: center;
    padding: 20px 0 60px;
    position: relative;
  }
  .hero-kicker {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 32px;
  }
  .hero-kicker span { color: var(--ink-mute); }
  .hero-label {
    font-family: 'Instrument Sans', sans-serif;
    font-size: 18px;
    color: var(--ink-soft);
    margin-bottom: 18px;
    font-weight: 400;
  }
  .hero-amount {
    font-family: 'Fraunces', serif;
    font-weight: 400;
    font-variation-settings: "opsz" 144, "SOFT" 50;
    font-size: clamp(72px, 14vw, 200px);
    line-height: 0.92;
    letter-spacing: -0.04em;
    background: var(--grad-savings);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    margin-bottom: 24px;
    font-style: italic;
    display: inline-block;
    padding: 0 10px;
  }
  .hero-amount .unit {
    font-family: 'Instrument Sans', sans-serif;
    font-size: 0.25em;
    font-weight: 500;
    font-style: normal;
    letter-spacing: 0;
    vertical-align: 0.4em;
    background: var(--grad-savings);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
  }
  .hero-caption {
    font-family: 'Fraunces', serif;
    font-size: clamp(18px, 2.2vw, 24px);
    color: var(--ink);
    max-width: 640px;
    margin: 0 auto;
    line-height: 1.4;
    font-weight: 400;
  }
  .hero-caption em {
    font-style: italic;
    color: var(--accent);
  }
  .hero-pct {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    margin-top: 28px;
    padding: 8px 16px;
    border: 1px solid var(--line);
    border-radius: 100px;
    background: var(--bg-panel);
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    color: var(--ok);
    font-weight: 500;
  }
  .hero-pct::before {
    content: '↓';
    font-size: 14px;
  }

  /* ─── Calculator Grid ─────────────────────────────────── */
  .calc {
    display: grid;
    grid-template-columns: 380px 1fr;
    gap: 40px;
    margin-bottom: 72px;
  }

  @media (max-width: 900px) {
    .calc { grid-template-columns: 1fr; gap: 32px; }
    .wrap { padding: 32px 20px 60px; }
  }

  /* ─── Inputs Panel ────────────────────────────────────── */
  .inputs {
    background: var(--bg-panel);
    border: 1px solid var(--line);
    border-radius: 4px;
    padding: 32px;
    box-shadow: var(--shadow-sm);
    position: sticky;
    top: 24px;
    align-self: start;
    height: fit-content;
  }
  .inputs-title {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--ink-mute);
    margin-bottom: 4px;
  }
  .inputs-subtitle {
    font-family: 'Fraunces', serif;
    font-size: 22px;
    margin-bottom: 28px;
    font-weight: 500;
    letter-spacing: -0.01em;
  }

  .field {
    margin-bottom: 22px;
  }
  .field-label {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 8px;
  }
  .field-name {
    font-size: 13px;
    color: var(--ink);
    font-weight: 500;
  }
  .field-value {
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    color: var(--accent);
    font-weight: 500;
  }
  .field-hint {
    font-size: 11px;
    color: var(--ink-mute);
    margin-top: 4px;
    font-style: italic;
  }

  select, input[type="range"], input[type="number"] {
    font-family: inherit;
    font-size: 14px;
  }

  select {
    width: 100%;
    padding: 10px 12px;
    background: var(--bg-card);
    border: 1px solid var(--line);
    border-radius: 2px;
    color: var(--ink);
    cursor: pointer;
    transition: border-color 0.15s;
    font-weight: 500;
  }
  select:hover, select:focus {
    border-color: var(--accent);
    outline: none;
  }

  input[type="range"] {
    width: 100%;
    -webkit-appearance: none;
    appearance: none;
    background: transparent;
    cursor: pointer;
  }
  input[type="range"]::-webkit-slider-runnable-track {
    height: 4px;
    background: linear-gradient(to right, var(--accent) 0%, var(--accent) var(--pct, 50%), var(--line) var(--pct, 50%), var(--line) 100%);
    border-radius: 2px;
  }
  input[type="range"]::-moz-range-track {
    height: 4px;
    background: var(--line);
    border-radius: 2px;
  }
  input[type="range"]::-webkit-slider-thumb {
    -webkit-appearance: none;
    height: 16px;
    width: 16px;
    background: var(--bg-card);
    border: 2px solid var(--accent);
    border-radius: 50%;
    margin-top: -6px;
    cursor: grab;
    transition: transform 0.1s;
  }
  input[type="range"]::-webkit-slider-thumb:hover {
    transform: scale(1.15);
  }
  input[type="range"]::-webkit-slider-thumb:active { cursor: grabbing; }
  input[type="range"]::-moz-range-thumb {
    height: 16px;
    width: 16px;
    background: var(--bg-card);
    border: 2px solid var(--accent);
    border-radius: 50%;
    cursor: pointer;
  }

  .toggle-row {
    display: flex;
    gap: 8px;
    padding: 6px;
    background: var(--line-soft);
    border-radius: 2px;
  }
  .toggle-btn {
    flex: 1;
    padding: 10px 12px;
    background: transparent;
    border: none;
    font-family: inherit;
    font-size: 12px;
    font-weight: 500;
    color: var(--ink-soft);
    cursor: pointer;
    border-radius: 2px;
    transition: all 0.15s;
    letter-spacing: 0.03em;
  }
  .toggle-btn.active {
    background: var(--bg-card);
    color: var(--accent);
    box-shadow: var(--shadow-sm);
  }

  /* ─── Scenarios Panel ─────────────────────────────────── */
  .scenarios {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  .scenario {
    background: var(--bg-card);
    border: 1px solid var(--line);
    border-radius: 4px;
    padding: 28px 32px;
    position: relative;
    overflow: hidden;
    transition: all 0.2s;
  }

  .scenario.featured {
    border: 1px solid var(--accent);
    box-shadow: var(--shadow-lg);
    padding-top: 36px;
  }
  .scenario.featured::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: var(--grad-hero);
  }

  .scenario-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 16px;
    gap: 20px;
  }
  .scenario-tag {
    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    padding: 4px 10px;
    border-radius: 100px;
    display: inline-block;
    margin-bottom: 10px;
    font-weight: 500;
  }
  .scenario-a .scenario-tag { background: #FEE2E2; color: var(--bad); }
  .scenario-b .scenario-tag { background: var(--line-soft); color: var(--ink-soft); }
  .scenario-c .scenario-tag { background: #D1FAE5; color: var(--ok); }

  .scenario-name {
    font-family: 'Fraunces', serif;
    font-size: 22px;
    font-weight: 500;
    letter-spacing: -0.01em;
    line-height: 1.25;
  }
  .scenario-name em {
    font-style: italic;
    color: var(--accent);
  }
  .scenario-desc {
    font-size: 14px;
    color: var(--ink-soft);
    margin-top: 6px;
    max-width: 380px;
  }

  .scenario-cost {
    text-align: right;
    flex-shrink: 0;
  }
  .cost-amount {
    font-family: 'Fraunces', serif;
    font-size: 44px;
    font-weight: 400;
    letter-spacing: -0.03em;
    line-height: 1;
    font-variation-settings: "opsz" 96;
  }
  .scenario.featured .cost-amount {
    background: var(--grad-hero);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    font-style: italic;
  }
  .cost-unit {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: var(--ink-mute);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-top: 6px;
  }

  .scenario-bar {
    height: 8px;
    background: var(--line-soft);
    border-radius: 4px;
    overflow: hidden;
    margin-top: 16px;
  }
  .scenario-bar-fill {
    height: 100%;
    border-radius: 4px;
    transition: width 0.5s cubic-bezier(0.22, 1, 0.36, 1);
  }
  .scenario-a .scenario-bar-fill { background: linear-gradient(90deg, #B91C1C, #DC2626); }
  .scenario-b .scenario-bar-fill { background: linear-gradient(90deg, #A8A29E, #78716C); }
  .scenario-c .scenario-bar-fill { background: var(--grad-hero); }

  .scenario-breakdown {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 14px;
    margin-top: 20px;
    padding-top: 16px;
    border-top: 1px dashed var(--line);
  }
  .breakdown-item {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
  }
  .breakdown-label {
    color: var(--ink-mute);
    text-transform: uppercase;
    letter-spacing: 0.08em;
    margin-bottom: 3px;
    font-size: 10px;
  }
  .breakdown-val {
    color: var(--ink);
    font-weight: 500;
    font-size: 13px;
  }

  /* ─── Bottom Stats ────────────────────────────────────── */
  .stats {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--line);
    border: 1px solid var(--line);
    border-radius: 4px;
    margin-bottom: 60px;
    overflow: hidden;
  }
  @media (max-width: 720px) {
    .stats { grid-template-columns: 1fr; }
  }
  .stat {
    background: var(--bg-card);
    padding: 28px 32px;
  }
  .stat-label {
    font-family: 'JetBrains Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--ink-mute);
    margin-bottom: 12px;
  }
  .stat-value {
    font-family: 'Fraunces', serif;
    font-size: 38px;
    font-weight: 400;
    letter-spacing: -0.02em;
    line-height: 1;
    margin-bottom: 6px;
  }
  .stat-value.accent {
    background: var(--grad-hero);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    font-style: italic;
  }
  .stat-caption {
    font-size: 12px;
    color: var(--ink-soft);
    line-height: 1.4;
  }

  /* ─── Footnote ────────────────────────────────────────── */
  .footnote {
    max-width: 740px;
    margin: 0 auto;
    text-align: center;
    padding-top: 48px;
    border-top: 1px solid var(--line);
  }
  .footnote-title {
    font-family: 'Fraunces', serif;
    font-style: italic;
    font-size: 20px;
    margin-bottom: 14px;
    color: var(--ink);
  }
  .footnote-body {
    font-size: 13px;
    color: var(--ink-soft);
    line-height: 1.7;
  }
  .footnote-body a {
    color: var(--accent);
    text-decoration: none;
    border-bottom: 1px solid currentColor;
  }

  /* ─── Pricing Reference Table ─────────────────────────── */
  .pricing-ref {
    margin-top: 48px;
    padding: 28px 32px;
    background: var(--bg-panel);
    border: 1px solid var(--line);
    border-radius: 4px;
  }
  .pricing-ref-title {
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--ink-mute);
    margin-bottom: 18px;
  }
  .pricing-table {
    width: 100%;
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    border-collapse: collapse;
  }
  .pricing-table th {
    text-align: left;
    font-weight: 500;
    color: var(--ink-mute);
    padding: 8px 12px 8px 0;
    letter-spacing: 0.04em;
    font-size: 10px;
    text-transform: uppercase;
    border-bottom: 1px solid var(--line);
  }
  .pricing-table th:not(:first-child), .pricing-table td:not(:first-child) {
    text-align: right;
  }
  .pricing-table td {
    padding: 10px 12px 10px 0;
    border-bottom: 1px solid var(--line-soft);
    color: var(--ink);
  }
  .pricing-table td:first-child { font-weight: 500; }
  .pricing-table tr:last-child td { border-bottom: none; }

  /* Small screens refinements */
  @media (max-width: 600px) {
    .scenario-header { flex-direction: column; gap: 14px; }
    .scenario-cost { text-align: left; }
    .cost-amount { font-size: 36px; }
    .inputs { padding: 24px; }
    .scenario { padding: 22px 24px; }
  }
</style>
</head>
<body>

<div class="wrap">

  <header>
    <div class="brand">Context Engineering Kit</div>
    <div class="header-meta">Cost Calculator · v1.0 · Apr 2026</div>
  </header>

  <section class="hero">
    <div class="hero-kicker">Your Estimated Monthly Savings <span>— with persistent context + prompt caching</span></div>
    <div class="hero-amount" id="heroAmount">$0<span class="unit">/mo</span></div>
    <div class="hero-caption">
      That's <em id="heroAnnual">$0/year</em> you keep by treating context as infrastructure, not chat history.
    </div>
    <div class="hero-pct" id="heroPct">0% vs. baseline</div>
  </section>

  <section class="calc">

    <!-- ───── Inputs Panel ───── -->
    <aside class="inputs">
      <div class="inputs-title">Configure</div>
      <div class="inputs-subtitle">Your AI operation</div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Model</span>
          <span class="field-value" id="modelPrice">—</span>
        </div>
        <select id="model">
          <option value="claude-opus-4.7">Claude Opus 4.7</option>
          <option value="claude-sonnet-4.6" selected>Claude Sonnet 4.6</option>
          <option value="claude-haiku-4.5">Claude Haiku 4.5</option>
          <option value="gpt-5.4">GPT-5.4</option>
          <option value="gpt-5.2">GPT-5.2</option>
          <option value="gemini-3.1-pro">Gemini 3.1 Pro</option>
          <option value="gemini-3-flash">Gemini 3 Flash</option>
        </select>
        <div class="field-hint">Input / output price per million tokens</div>
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Agents</span>
          <span class="field-value" id="agentsVal">10</span>
        </div>
        <input type="range" id="agents" min="1" max="50" value="10" step="1">
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Sessions / day / agent</span>
          <span class="field-value" id="sessionsVal">40</span>
        </div>
        <input type="range" id="sessions" min="1" max="200" value="40" step="1">
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Context size</span>
          <span class="field-value" id="contextVal">6,000 tok</span>
        </div>
        <input type="range" id="context" min="1000" max="30000" value="6000" step="500">
        <div class="field-hint">Your .md persona + rules + knowledge base</div>
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Conv. input / session</span>
          <span class="field-value" id="convVal">500 tok</span>
        </div>
        <input type="range" id="conv" min="100" max="5000" value="500" step="50">
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Output / session</span>
          <span class="field-value" id="outputVal">500 tok</span>
        </div>
        <input type="range" id="output" min="100" max="5000" value="500" step="50">
      </div>

      <div class="field">
        <div class="field-label">
          <span class="field-name">Caching</span>
        </div>
        <div class="toggle-row">
          <button type="button" class="toggle-btn active" data-cache="on">Prompt cache ON</button>
          <button type="button" class="toggle-btn" data-cache="off">OFF</button>
        </div>
        <div class="field-hint">Affects Scenario C only · ~90% discount on cached prefix reads</div>
      </div>
    </aside>

    <!-- ───── Scenarios ───── -->
    <div class="scenarios">

      <div class="scenario scenario-a">
        <div class="scenario-header">
          <div>
            <div class="scenario-tag">Scenario A · Baseline</div>
            <div class="scenario-name">No context file</div>
            <div class="scenario-desc">Re-explain project every session. Extra clarification turns eat tokens on both sides.</div>
          </div>
          <div class="scenario-cost">
            <div class="cost-amount" id="costA">$—</div>
            <div class="cost-unit">/ month</div>
          </div>
        </div>
        <div class="scenario-bar"><div class="scenario-bar-fill" id="barA" style="width:100%"></div></div>
        <div class="scenario-breakdown">
          <div class="breakdown-item">
            <div class="breakdown-label">Input tokens</div>
            <div class="breakdown-val" id="aInput">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">Output tokens</div>
            <div class="breakdown-val" id="aOutput">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">Overhead</div>
            <div class="breakdown-val" style="color:var(--bad)">+50% tokens</div>
          </div>
        </div>
      </div>

      <div class="scenario scenario-b">
        <div class="scenario-header">
          <div>
            <div class="scenario-tag">Scenario B · Midway</div>
            <div class="scenario-name">.md context, <em>no caching</em></div>
            <div class="scenario-desc">Stable prefix loaded every session, but no API-level cache discount applied.</div>
          </div>
          <div class="scenario-cost">
            <div class="cost-amount" id="costB">$—</div>
            <div class="cost-unit">/ month</div>
          </div>
        </div>
        <div class="scenario-bar"><div class="scenario-bar-fill" id="barB" style="width:80%"></div></div>
        <div class="scenario-breakdown">
          <div class="breakdown-item">
            <div class="breakdown-label">Input tokens</div>
            <div class="breakdown-val" id="bInput">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">Output tokens</div>
            <div class="breakdown-val" id="bOutput">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">vs. Scenario A</div>
            <div class="breakdown-val" id="bSave">—</div>
          </div>
        </div>
      </div>

      <div class="scenario scenario-c featured">
        <div class="scenario-header">
          <div>
            <div class="scenario-tag">Scenario C · Recommended</div>
            <div class="scenario-name">.md context <em>+ prompt caching</em></div>
            <div class="scenario-desc">Context file loaded as cached prefix — ~90% off on every session after the first write.</div>
          </div>
          <div class="scenario-cost">
            <div class="cost-amount" id="costC">$—</div>
            <div class="cost-unit">/ month</div>
          </div>
        </div>
        <div class="scenario-bar"><div class="scenario-bar-fill" id="barC" style="width:30%"></div></div>
        <div class="scenario-breakdown">
          <div class="breakdown-item">
            <div class="breakdown-label">Cache writes</div>
            <div class="breakdown-val" id="cWrite">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">Cache reads (90% off)</div>
            <div class="breakdown-val" id="cRead">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">Output</div>
            <div class="breakdown-val" id="cOutput">—</div>
          </div>
          <div class="breakdown-item">
            <div class="breakdown-label">vs. Scenario A</div>
            <div class="breakdown-val" id="cSave" style="color:var(--ok)">—</div>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- ───── Bottom Stats ───── -->
  <section class="stats">
    <div class="stat">
      <div class="stat-label">Annual savings</div>
      <div class="stat-value accent" id="statYear">$0</div>
      <div class="stat-caption">Scenario A → C, at your current settings</div>
    </div>
    <div class="stat">
      <div class="stat-label">Per-agent savings</div>
      <div class="stat-value" id="statAgent">$0</div>
      <div class="stat-caption">Monthly savings divided across your agents</div>
    </div>
    <div class="stat">
      <div class="stat-label">Sessions this month</div>
      <div class="stat-value" id="statSessions">0</div>
      <div class="stat-caption">Total across all agents in 30 days</div>
    </div>
  </section>

  <!-- ───── Pricing Reference ───── -->
  <div class="pricing-ref">
    <div class="pricing-ref-title">Pricing reference · per million tokens · April 2026</div>
    <table class="pricing-table">
      <thead>
        <tr>
          <th>Model</th>
          <th>Input</th>
          <th>Output</th>
          <th>Cache Read</th>
          <th>Cache Write</th>
        </tr>
      </thead>
      <tbody id="priceTable"></tbody>
    </table>
  </div>

  <!-- ───── Footnote ───── -->
  <div class="footnote">
    <div class="footnote-title">Methodology</div>
    <div class="footnote-body">
      Scenario A assumes the user re-types partial context each session and triggers clarification turns, modeled as a 50% token overhead on input and 20% on output. Scenario B loads a persistent <code>.md</code> prefix but without API-level caching. Scenario C enables Anthropic-style prompt caching (cache writes at 1.25× input, cache reads at 0.10× input), with one cache write per agent per day and the rest amortized across reads. Actual savings vary by cache hit rate, session burstiness, and model-specific caching policies. Pricing compiled from official Anthropic, OpenAI, and Google pricing pages as of April 2026.
      <br><br>
      Part of the <a href="#">Context Engineering Kit</a>. MIT licensed.
    </div>
  </div>

</div>

<script>
  // ─── Pricing data (USD per million tokens, April 2026) ───
  const MODELS = {
    'claude-opus-4.7':   { name: 'Claude Opus 4.7',    input: 5.00,  output: 25.00, cacheRead: 0.50,  cacheWrite: 6.25 },
    'claude-sonnet-4.6': { name: 'Claude Sonnet 4.6',  input: 3.00,  output: 15.00, cacheRead: 0.30,  cacheWrite: 3.75 },
    'claude-haiku-4.5':  { name: 'Claude Haiku 4.5',   input: 1.00,  output: 5.00,  cacheRead: 0.10,  cacheWrite: 1.25 },
    'gpt-5.4':           { name: 'GPT-5.4',            input: 2.50,  output: 20.00, cacheRead: 0.25,  cacheWrite: 2.50 },
    'gpt-5.2':           { name: 'GPT-5.2',            input: 1.75,  output: 14.00, cacheRead: 0.18,  cacheWrite: 1.75 },
    'gemini-3.1-pro':    { name: 'Gemini 3.1 Pro',     input: 2.00,  output: 12.00, cacheRead: 0.20,  cacheWrite: 2.50 },
    'gemini-3-flash':    { name: 'Gemini 3 Flash',     input: 0.50,  output: 3.00,  cacheRead: 0.05,  cacheWrite: 0.625 },
  };

  const DAYS = 30;
  const M = 1_000_000;

  // ─── Format helpers ───
  const fmt$ = (n) => {
    if (n >= 10000) return '$' + (n / 1000).toFixed(1) + 'K';
    if (n >= 1000)  return '$' + Math.round(n).toLocaleString();
    if (n >= 100)   return '$' + Math.round(n).toLocaleString();
    if (n >= 10)    return '$' + n.toFixed(0);
    return '$' + n.toFixed(2);
  };
  const fmt$full = (n) => '$' + Math.round(n).toLocaleString();
  const fmtTok = (n) => {
    if (n >= 1e9) return (n / 1e9).toFixed(2) + 'B';
    if (n >= 1e6) return (n / 1e6).toFixed(1) + 'M';
    if (n >= 1e3) return (n / 1e3).toFixed(0) + 'K';
    return n.toLocaleString();
  };

  // ─── Calculation ───
  function calculate(inputs, model, cacheOn) {
    const { agents, sessionsPerDay, contextTokens, convInputTokens, outputTokens } = inputs;
    const totalSessions = agents * sessionsPerDay * DAYS;

    // Scenario A — no context file, re-explain each time + clarification overhead
    const aInputTokens = totalSessions * (contextTokens * 1.5 + convInputTokens);
    const aOutputTokens = totalSessions * outputTokens * 1.2;
    const aCost = (aInputTokens * model.input + aOutputTokens * model.output) / M;

    // Scenario B — .md context, no caching
    const bInputTokens = totalSessions * (contextTokens + convInputTokens);
    const bOutputTokens = totalSessions * outputTokens;
    const bCost = (bInputTokens * model.input + bOutputTokens * model.output) / M;

    // Scenario C — .md context + caching (if cacheOn; otherwise same as B)
    let cCost, cacheWrites, cacheReadTokens, cacheWriteTokens, cOutputCost, cConvInputCost;
    if (cacheOn) {
      cacheWrites = agents * DAYS;
      const cacheReads = totalSessions - cacheWrites;
      cacheWriteTokens = cacheWrites * contextTokens;
      cacheReadTokens = cacheReads * contextTokens;
      const cWriteCost = cacheWriteTokens * model.cacheWrite / M;
      const cReadCost = cacheReadTokens * model.cacheRead / M;
      cConvInputCost = totalSessions * convInputTokens * model.input / M;
      cOutputCost = totalSessions * outputTokens * model.output / M;
      cCost = cWriteCost + cReadCost + cConvInputCost + cOutputCost;
    } else {
      cCost = bCost;
      cacheWrites = 0;
      cacheReadTokens = 0;
      cacheWriteTokens = 0;
      cOutputCost = bOutputTokens * model.output / M;
      cConvInputCost = totalSessions * convInputTokens * model.input / M;
    }

    return {
      totalSessions,
      a: { cost: aCost, input: aInputTokens, output: aOutputTokens },
      b: { cost: bCost, input: bInputTokens, output: bOutputTokens },
      c: { cost: cCost, cacheWrites, cacheReadTokens, cacheWriteTokens, outputCost: cOutputCost, convInputCost: cConvInputCost },
    };
  }

  // ─── UI wiring ───
  const $ = (id) => document.getElementById(id);
  const state = {
    agents: 10,
    sessionsPerDay: 40,
    contextTokens: 6000,
    convInputTokens: 500,
    outputTokens: 500,
    modelKey: 'claude-sonnet-4.6',
    cacheOn: true,
  };

  function readInputs() {
    state.agents = parseInt($('agents').value);
    state.sessionsPerDay = parseInt($('sessions').value);
    state.contextTokens = parseInt($('context').value);
    state.convInputTokens = parseInt($('conv').value);
    state.outputTokens = parseInt($('output').value);
    state.modelKey = $('model').value;
  }

  function updateLabels() {
    $('agentsVal').textContent = state.agents;
    $('sessionsVal').textContent = state.sessionsPerDay;
    $('contextVal').textContent = state.contextTokens.toLocaleString() + ' tok';
    $('convVal').textContent = state.convInputTokens.toLocaleString() + ' tok';
    $('outputVal').textContent = state.outputTokens.toLocaleString() + ' tok';
    const m = MODELS[state.modelKey];
    $('modelPrice').textContent = `$${m.input}/$${m.output}`;

    // Update slider fill gradients
    const sliders = [
      { el: $('agents'), min: 1, max: 50 },
      { el: $('sessions'), min: 1, max: 200 },
      { el: $('context'), min: 1000, max: 30000 },
      { el: $('conv'), min: 100, max: 5000 },
      { el: $('output'), min: 100, max: 5000 },
    ];
    sliders.forEach(({ el, min, max }) => {
      const pct = ((el.value - min) / (max - min)) * 100;
      el.style.setProperty('--pct', pct + '%');
    });
  }

  function render() {
    readInputs();
    updateLabels();
    const model = MODELS[state.modelKey];
    const r = calculate(state, model, state.cacheOn);

    // Hero
    const saved = r.a.cost - r.c.cost;
    const pct = r.a.cost > 0 ? Math.round((saved / r.a.cost) * 100) : 0;
    $('heroAmount').innerHTML = fmt$(saved) + '<span class="unit">/mo</span>';
    $('heroAnnual').textContent = fmt$full(saved * 12) + '/year';
    $('heroPct').textContent = `${pct}% vs. baseline`;

    // Scenario A
    $('costA').textContent = fmt$(r.a.cost);
    $('aInput').textContent = fmtTok(r.a.input);
    $('aOutput').textContent = fmtTok(r.a.output);

    // Scenario B
    $('costB').textContent = fmt$(r.b.cost);
    $('bInput').textContent = fmtTok(r.b.input);
    $('bOutput').textContent = fmtTok(r.b.output);
    const bSave = r.a.cost - r.b.cost;
    const bSavePct = r.a.cost > 0 ? Math.round((bSave / r.a.cost) * 100) : 0;
    $('bSave').textContent = bSave > 0 ? `−${bSavePct}% (${fmt$(bSave)})` : '—';

    // Scenario C
    $('costC').textContent = fmt$(r.c.cost);
    if (state.cacheOn) {
      $('cWrite').textContent = `${r.c.cacheWrites} × ${state.contextTokens.toLocaleString()} tok`;
      $('cRead').textContent = fmtTok(r.c.cacheReadTokens);
    } else {
      $('cWrite').textContent = 'disabled';
      $('cRead').textContent = 'disabled';
    }
    $('cOutput').textContent = fmtTok(r.b.output);
    const cSavePct = r.a.cost > 0 ? Math.round((saved / r.a.cost) * 100) : 0;
    $('cSave').textContent = saved > 0 ? `−${cSavePct}% (${fmt$(saved)})` : '—';

    // Bars (relative to A)
    const maxCost = r.a.cost;
    if (maxCost > 0) {
      $('barA').style.width = '100%';
      $('barB').style.width = ((r.b.cost / maxCost) * 100) + '%';
      $('barC').style.width = ((r.c.cost / maxCost) * 100) + '%';
    }

    // Stats
    $('statYear').textContent = fmt$full(saved * 12);
    $('statAgent').textContent = state.agents > 0 ? fmt$(saved / state.agents) : '$0';
    $('statSessions').textContent = r.totalSessions.toLocaleString();
  }

  // ─── Event listeners ───
  ['agents', 'sessions', 'context', 'conv', 'output', 'model'].forEach(id => {
    $(id).addEventListener('input', render);
  });
  document.querySelectorAll('.toggle-btn').forEach(btn => {
    btn.addEventListener('click', () => {
      document.querySelectorAll('.toggle-btn').forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      state.cacheOn = btn.dataset.cache === 'on';
      render();
    });
  });

  // ─── Build pricing reference table ───
  const tbody = $('priceTable');
  Object.entries(MODELS).forEach(([key, m]) => {
    const tr = document.createElement('tr');
    tr.innerHTML = `
      <td>${m.name}</td>
      <td>$${m.input.toFixed(2)}</td>
      <td>$${m.output.toFixed(2)}</td>
      <td>$${m.cacheRead.toFixed(2)}</td>
      <td>$${m.cacheWrite.toFixed(2)}</td>
    `;
    tbody.appendChild(tr);
  });

  // Initial render
  render();
</script>

</body>
</html>
