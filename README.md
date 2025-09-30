<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portfolio — Pavan Khakre</title>
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#f9fbfc;
      --card:#ffffff;
      --accent:#2563eb;
      --muted:#4b5563;
      --glass: rgba(37,99,235,0.08);
      --radius:14px;
      --max-width:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background:var(--bg);
      color:#1f2937;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:32px 16px;
      display:flex;
      justify-content:center;
    }
    .container{
      width:100%;
      max-width:var(--max-width);
      background: var(--card);
      border-radius:20px;
      padding:28px;
      box-shadow:0 6px 30px rgba(0,0,0,0.08);
    }

    header{
      display:flex;align-items:center;justify-content:space-between;margin-bottom:18px;
    }
    .brand{display:flex;align-items:center;gap:12px}
    .avatar{
      width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#60a5fa);display:flex;align-items:center;justify-content:center;font-weight:700;color:#fff
    }
    h1{margin:0;font-size:1.25rem;color:#111827}
    nav{display:flex;gap:12px}
    nav a{color:var(--muted);text-decoration:none;padding:8px 10px;border-radius:8px;font-weight:500}
    nav a:hover{color:var(--accent);background:var(--glass)}

    main{display:grid;grid-template-columns:1fr 360px;gap:20px}

    .card{background:var(--card);border-radius:var(--radius);padding:18px;border:1px solid #e5e7eb}

    .hero{display:flex;flex-direction:column;gap:10px}
    .hero p{margin:0;color:var(--muted)}

    .skills{display:grid;grid-template-columns:repeat(2,1fr);gap:10px;margin-top:12px}
    .skill{background:#f3f4f6;padding:12px;border-radius:12px}
    .skill h4{margin:0 0 8px 0;font-size:0.95rem;color:#111827}
    .skill .bar{height:10px;background:#e5e7eb;border-radius:999px;overflow:hidden}
    .skill .bar > span{display:block;height:100%;border-radius:999px;background:linear-gradient(90deg,var(--accent),#60a5fa)}

    .experience{margin-top:12px}
    .exp-item{display:flex;gap:12px;padding:12px;background:#f9fafb;border-radius:12px;margin-bottom:10px;border:1px solid #e5e7eb}
    .exp-item .meta{min-width:110px;color:var(--muted);font-size:0.9rem}
    .exp-item .body h4{margin:0 0 6px 0;color:#111827}
    .exp-item .body p{margin:0;color:var(--muted);font-size:0.95rem}

    .profile{display:flex;flex-direction:column;gap:12px}
    .contact-card{display:flex;flex-direction:column;gap:8px}
    label{font-size:0.85rem;color:var(--muted)}
    input,textarea{padding:10px;border-radius:10px;border:1px solid #d1d5db;background:#fff;color:#111827}
    .btn{display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#60a5fa);color:#fff;font-weight:600;border:none;cursor:pointer}

    footer{margin-top:16px;padding-top:12px;border-top:1px solid #e5e7eb;display:flex;justify-content:space-between;color:var(--muted);font-size:0.9rem}

    @media (max-width:900px){
      main{grid-template-columns:1fr}
      .avatar{width:48px;height:48px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="avatar" style="background-image:url('my\ photo.jpg'); background-size:cover; background-position:center;"></div>
        <div>
          <h1>Pavan Shivaji Khakre</h1>
          <div style="color:var(--muted);font-size:0.9rem">BSc Computer Science Student • Web Developer • Software Enthusiast</div>
        </div>
      </div>
      <nav>
        <a href="#bio">Bio</a>
        <a href="#skills">Skills</a>
        <a href="#education">Education</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section>
        <article class="card hero" id="bio">
          <h2>About Me</h2>
          <p>I am a <strong>BSc Computer Science</strong> student passionate about building modern web applications and exploring software engineering concepts. Skilled in HTML, CSS, JavaScript, and Java, with a foundation in Data Structures & Algorithms. I enjoy solving coding challenges, learning new tools, and collaborating on projects. My career goal is to grow into a full-stack developer and contribute to impactful software solutions.</p>
        </article>

        <article class="card" id="skills" style="margin-top:14px">
          <h3>Technical Skills</h3>
          <div class="skills">
            <div class="skill">
              <h4>HTML & CSS</h4>
              <div class="bar"><span style="width:90%"></span></div>
            </div>
            <div class="skill">
              <h4>JavaScript</h4>
              <div class="bar"><span style="width:80%"></span></div>
            </div>
            <div class="skill">
              <h4>Java</h4>
              <div class="bar"><span style="width:75%"></span></div>
            </div>
            <div class="skill">
              <h4>C / C++</h4>
              <div class="bar"><span style="width:70%"></span></div>
            </div>
            <div class="skill">
              <h4>Data Structures & Algorithms</h4>
              <div class="bar"><span style="width:65%"></span></div>
            </div>
            <div class="skill">
              <h4>Git & VS Code</h4>
              <div class="bar"><span style="width:85%"></span></div>
            </div>
          </div>
        </article>

        <article class="card experience" id="education">
          <h3>Education</h3>
          <div class="exp-item">
            <div class="meta">2023 – 2026</div>
            <div class="body">
              <h4>Bachelor of Science in Computer Science</h4>
              <p>Modern College of Arts, Science and Commerce, Ganeshkhind, Pune, Maharashtra</p>
            </div>
          </div>
          <div class="exp-item">
            <div class="meta">2021 – 2022</div>
            <div class="body">
              <h4>HSC — 81%</h4>
              <p>Vinay Vidhyalay Jalgaon (S), Jalna, Maharashtra</p>
            </div>
          </div>
          <div class="exp-item">
            <div class="meta">2019 – 2020</div>
            <div class="body">
              <h4>SSC — 75%</h4>
              <p>D B Ghumare Public School, Beed, Maharashtra</p>
            </div>
          </div>
        </article>

        <article class="card" style="margin-top:14px">
          <h3>Certifications</h3>
          <ul style="color:var(--muted)">
            <li>MS-CIT</li>
            <li>Typing 30 English</li>
          </ul>
        </article>
      </section>

      <aside class="profile">
        <div class="card contact-card" id="contact">
          <h3>Contact</h3>
          <p style="color:var(--muted);margin:0">Feel free to reach out!</p>

          <p style="margin:6px 0">📧 <a href="mailto:pavankhakre1013@gmail.com" style="color:var(--accent);text-decoration:none">pavankhakre1013@gmail.com</a></p>
          <p style="margin:6px 0">📱 +91 7038902645</p>
          <p style="margin:6px 0">💼 <a href="https://www.linkedin.com/in/pavan-khakre-375b322a2" target="_blank" style="color:var(--accent);text-decoration:none">LinkedIn Profile</a></p>
        </div>
      </aside>
    </main>

    <footer>
      <div>© <span id="year"></span> Pavan Khakre</div>
      <div>Built with ❤️ • <a href="#bio" style="color:var(--accent);text-decoration:none">Back to top</a></div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
