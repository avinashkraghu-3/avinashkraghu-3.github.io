<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ethical Hacking & Cybersecurity — Resources & Awareness</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#06b6d4; --glass: rgba(255,255,255,0.03);
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg,#071022 0%, #071520 60%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:32px;
    }
    .wrap{max-width:var(--maxw); margin:0 auto;}
    header{display:flex; align-items:center; justify-content:space-between; gap:16px; margin-bottom:26px}
    .brand{display:flex; align-items:center; gap:12px}
    .logo{
      width:56px; height:56px; border-radius:10px;
      background:linear-gradient(135deg,var(--accent), #3b82f6);
      display:flex; align-items:center; justify-content:center; font-weight:700; color:#041025;
      box-shadow:0 6px 18px rgba(3,7,18,0.6);
    }
    h1{margin:0; font-size:20px}
    p.lead{margin:6px 0 0; color:var(--muted); font-size:14px}

    main{display:grid; grid-template-columns: 1fr 360px; gap:22px;}
    .card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:12px; padding:18px; box-shadow:0 6px 18px rgba(2,6,23,0.6); border:1px solid rgba(255,255,255,0.03)
    }
    .hero{padding:28px}
    .hero h2{margin:0 0 8px; font-size:26px}
    .hero p{color:var(--muted); margin:0 0 18px}
    .badges{display:flex; gap:8px; flex-wrap:wrap}
    .badge{background:var(--glass); padding:8px 10px; border-radius:999px; color:var(--muted); font-size:13px}

    section h3{margin:0 0 10px; font-size:16px}
    ul.resources{padding-left:18px; margin:0; color:var(--muted)}
    ul.resources li{margin:8px 0}

    .panel{display:flex; flex-direction:column; gap:12px}
    .panel .small{font-size:13px; color:var(--muted)}

    footer{margin-top:20px; color:var(--muted); font-size:13px; text-align:center}
    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* responsive */
    @media (max-width:980px){
      main{grid-template-columns:1fr; padding-bottom:20px}
      .logo{width:48px;height:48px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">EH</div>
        <div>
          <h1>Ethical Hacking & Cybersecurity</h1>
          <p class="lead">Resources · Safe labs · Certifications · Legal & ethical guidance</p>
        </div>
      </div>
      <div class="badges">
        <div class="badge">Awareness</div>
        <div class="badge">Defensive Skills</div>
        <div class="badge">Safe Labs</div>
      </div>
    </header>

    <main>
      <div>
        <article class="card hero">
          <h2>Learn ethical hacking the right way</h2>
          <p>Ethical hacking is about understanding how systems fail so defenders can fix them. This page focuses on **legal**, **non-actionable** guidance: learning resources, safe practice environments, certifications, and how to protect systems — not how to break into them.</p>

          <section style="margin-top:18px">
            <h3>Core principles</h3>
            <ul class="resources">
              <li><strong>Consent first:</strong> only test systems you own or have explicit permission to test.</li>
              <li><strong>Document everything:</strong> keep records of tests, scope, and findings for transparency.</li>
              <li><strong>Responsible disclosure:</strong> report vulnerabilities to owners responsibly.</li>
              <li><strong>Privacy:</strong> never exfiltrate or publish sensitive user data.</li>
            </ul>
          </section>

          <section style="margin-top:16px">
            <h3>What to study (high-level)</h3>
            <ul class="resources">
              <li>Networking fundamentals (TCP/IP, DNS, HTTP/S)</li>
              <li>Operating systems (Linux internals, Windows fundamentals)</li>
              <li>Application security principles (authentication, access control, secure coding)</li>
              <li>Cryptography basics (hashes, symmetric/asymmetric encryption, TLS concepts)</li>
            </ul>
          </section>

          <section style="margin-top:16px">
            <h3>Safe practice labs & platforms</h3>
            <ul class="resources">
              <li>Use intentionally vulnerable training platforms (e.g. OWASP Juice Shop, Damn Vulnerable Web App) in isolated environments.</li>
              <li>Try Capture The Flag (CTF) challenges focused on learning, hosted by reputable organizers.</li>
              <li>Set up local VMs or containers to practice — never attack remote systems without permission.</li>
            </ul>
          </section>

          <section style="margin-top:16px">
            <h3>Certifications & learning paths</h3>
            <ul class="resources">
              <li>Beginner: CompTIA Security+</li>
              <li>Intermediate: eLearnSecurity / OSCP (penetration testing) — ensure lab ethics</li>
              <li>Specialist: Certified Cloud Security (specific cloud vendors)</li>
            </ul>
          </section>

        </article>

        <article class="card" style="margin-top:14px">
          <h3>Glossary (brief)</h3>
          <ul class="resources">
            <li><strong>Vulnerability</strong>: a weakness that can be exploited.</li>
            <li><strong>Exploit</strong>: a tool or technique that takes advantage of a vulnerability.</li>
            <li><strong>Threat actor</strong>: someone who poses risk (criminal, researcher, insider).</li>
          </ul>

          <h3 style="margin-top:12px">Responsible disclosure</h3>
          <p class="small">If you discover a vulnerability in a third-party product, follow the vendor's published disclosure policy or use a coordinated vulnerability disclosure program. Avoid public disclosure until the issue is fixed.</p>
        </article>
      </div>

      <aside>
        <div class="card panel">
          <div>
            <h3>Quick links</h3>
            <ul class="resources" style="margin-top:8px">
              <li><a href="https://owasp.org" target="_blank" rel="noopener">OWASP (Application security guidance)</a></li>
              <li><a href="https://www.cybersecurity.education" target="_blank" rel="noopener">Security learning hubs</a></li>
              <li><a href="https://ctftime.org" target="_blank" rel="noopener">CTFtime (events & challenges)</a></li>
            </ul>
          </div>

          <div>
            <h3 style="margin-top:12px">Tools (for defenders)</h3>
            <ul class="resources" style="margin-top:8px">
              <li>Network scanners (for asset inventory)</li>
              <li>Log management & SIEM (to detect attacks)</li>
              <li>Vulnerability scanners (to identify and patch weaknesses)</li>
            </ul>
          </div>

          <div style="margin-top:12px">
            <h3>Legal & ethical note</h3>
            <p class="small">This site promotes legal, ethical behavior. Unauthorized access to systems is illegal in most jurisdictions. Seek permission and consult legal guidance if unsure.</p>
          </div>
        </div>

        <div class="card" style="margin-top:14px">
          <h3>Get started (sandbox)</h3>
          <p class="small">To practice, create an isolated lab using virtual machines or container images, and use known vulnerable apps intentionally built for training. Keep your lab offline or on an isolated network.</p>
        </div>
      </aside>
    </main>

    <footer>
      <p>Created for education and awareness. Nothing here is intended to enable illegal activity.</p>
    </footer>
  </div>
</body>
</html>
