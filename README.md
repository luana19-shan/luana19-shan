<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tarjeta – Luana Flores</title>
  <style>
    :root { --bg:#0f172a; --fg:#e2e8f0; --card:#111827; --accent:#22d3ee; }
    [data-theme="light"]{ --bg:#f8fafc; --fg:#0f172a; --card:#ffffff; --accent:#0ea5e9; }
    *{ box-sizing:border-box; }
    body{ margin:0; font-family:system-ui,Segoe UI,Roboto,Ubuntu; background:var(--bg); color:var(--fg); display:grid; place-items:center; min-height:100vh; }
    .card{ width:min(560px,92%); background:var(--card); border:1px solid #33415533; border-radius:18px; padding:24px; box-shadow:0 10px 30px #00000033; }
    .title{ font-size:1.6rem; margin:0 0 8px; }
    .subtitle{ margin:0 0 16px; opacity:.9; }
    .badges{ display:flex; flex-wrap:wrap; gap:8px; margin:18px 0; }
    .badge{ padding:6px 10px; border-radius:999px; border:1px solid #33415555; font-size:.9rem; }
    .row{ display:flex; gap:12px; align-items:center; justify-content:space-between; margin-top:12px; }
    button{ cursor:pointer; padding:10px 14px; border-radius:12px; border:1px solid #33415555; background:transparent; color:var(--fg); }
    a{ color:var(--accent); text-decoration:none; }
  </style>
</head>
<body>
  <div class="card">
    <h1 class="title">Luana Flores</h1>
    <p class="subtitle">Front‑End Junior · Ingeniería de Software con IA</p>
    <div class="badges">
      <span class="badge">HTML</span>
      <span class="badge">CSS</span>
      <span class="badge">JavaScript</span>
      <span class="badge">React</span>
    </div>
    <p>Construyo interfaces accesibles y rápidas. Mira mis proyectos en <a href="#">GitHub</a>.</p>
    <div class="row">
      <small id="status">Tema: auto</small>
      <button id="toggle">Cambiar tema</button>
    </div>
  </div>
  <script>
    const root = document.documentElement;
    const key = 'luana-theme';
    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
    const saved = localStorage.getItem(key);
    function apply(theme){
      if(theme === 'light'){ root.setAttribute('data-theme','light'); }
      else if(theme === 'dark'){ root.removeAttribute('data-theme'); }
      else { prefersDark ? root.removeAttribute('data-theme') : root.setAttribute('data-theme','light'); }
      document.getElementById('status').textContent = `Tema: ${theme || 'auto'}`;
    }
    apply(saved);
    document.getElementById('toggle').addEventListener('click', ()=>{
      const next = saved === 'light' ? 'dark' : saved === 'dark' ? '' : 'light';
      localStorage.setItem(key, next);
      apply(next);
    });
  </script>
</body>
</html>

<!--
**luana19-shan/luana19-shan** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
