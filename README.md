<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Vijayabharathi — Profile</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--accent:#7dd3fc;--muted:#9aa4b2}
    *{box-sizing:border-box;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial}
    body{margin:0;background:linear-gradient(180deg,#071029 0%, #081224 100%);color:#e6eef6;display:flex;align-items:center;justify-content:center;height:100vh;padding:20px}
    .card{width:960px;max-width:100%;background:rgba(11,18,32,0.75);border-radius:14px;padding:26px;box-shadow:0 8px 30px rgba(2,6,23,0.6);display:grid;grid-template-columns:1fr 320px;gap:24px}
    header{display:flex;gap:16px;align-items:center}
    .avatar{width:88px;height:88px;border-radius:12px;background:linear-gradient(135deg,#023047,#065a82);display:flex;align-items:center;justify-content:center;font-weight:700;font-size:28px;color:var(--accent)}
    h1{margin:0;font-size:22px}
    .meta{color:var(--muted);margin-top:6px;font-size:14px}
    .section{background:rgba(255,255,255,0.02);padding:18px;border-radius:10px}
    .label{font-size:13px;color:var(--muted);margin-bottom:6px}
    .value{font-size:15px;margin-bottom:10px}
    .grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    a.link{color:var(--accent);text-decoration:none}
    footer{font-size:13px;color:var(--muted);padding-top:12px}
    .btn{display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,#0369a1,#0891b2);color:white;text-decoration:none;font-weight:600}
    @media (max-width:820px){.card{grid-template-columns:1fr;}
    .avatar{width:72px;height:72px}}
  </style>
</head>
<body>
  <main class="card">
    <section>
      <header>
        <div class="avatar">V</div>
        <div>
          <h1>Vijayabharathi</h1>
          <div class="meta">Job seeker • Virudunagar</div>
        </div>
      </header><div style="height:14px"></div>

  <div class="section">
    <div class="label">About Me</div>
    <div class="value">I am job seeker</div>
  </div>

  <div style="height:12px"></div>

  <div class="section">
    <div class="label">Personal details</div>
    <div class="grid">
      <div>
        <div class="label">Full name</div>
        <div class="value">Vijayabharathi</div>
      </div>
      <div>
        <div class="label">Date of birth</div>
        <div class="value">23/06/2005</div>
      </div>
      <div>
        <div class="label">Phone</div>
        <div class="value">+91 9384702148</div>
      </div>
      <div>
        <div class="label">Email</div>
        <div class="value"><a class="link" href="mailto:vijayabharathikaliraj@gmail.com">vijayabharathikaliraj@gmail.com</a></div>
      </div>
      <div style="grid-column:1/3">
        <div class="label">Location</div>
        <div class="value">Virudunagar</div>
      </div>
    </div>
  </div>

  <footer>
    <div>Tip: To make this shareable as a single link, host this file on GitHub Pages or Netlify. If you want, I can guide you step-by-step to publish it.</div>
  </footer>
</section>

<aside>
  <div class="section">
    <div class="label">Quick actions</div>
    <div style="margin-top:10px;display:flex;flex-direction:column;gap:10px">
      <a class="btn" href="mailto:vijayabharathikaliraj@gmail.com">Email</a>
      <a class="btn" href="#" onclick="copyProfile()">Copy contact</a>
      <a class="btn" href="#" onclick="downloadHTML()">Download .html</a>
    </div>
  </div>

  <div style="height:12px"></div>

  <div class="section">
    <div class="label">Privacy</div>
    <div class="value">You provided no photo. If you want to hide phone/email on public pages, tell me and I'll create a version without them.</div>
  </div>
</aside>

  </main>  <script>
    function copyProfile(){
      const text = `Name: Vijayabharathi\nDOB: 23/06/2005\nPhone: 9384702148\nEmail: vijayabharathikaliraj@gmail.com\nLocation: Virudunagar`;
      navigator.clipboard?.writeText(text).then(()=>alert('Contact copied to clipboard'))
    }

    function downloadHTML(){
      const content = document.documentElement.outerHTML;
      const blob = new Blob([content],{type:'text/html'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'Vijayabharathi_profile.html';
      a.click(); URL.revokeObjectURL(url);
    }
  </script></body>
</html>
