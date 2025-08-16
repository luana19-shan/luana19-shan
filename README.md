# ¡Hola! 👋

## Soy **Luana Flores**

### 👩‍💻 Programadora Front‑End Junior · Estudiante de **Ingeniería de Software con IA**

* ✨ Fuerte en **HTML**, **CSS** y **JavaScript** (vanilla).
* 🧠 Interesada en cómo la **IA** potencia el desarrollo front‑end (UX inteligente, componentes asistidos, automatización).
* 🧩 Me gusta escribir código limpio, accesible y bien documentado.
* 📍 Perú · Español (nativo)

> *Este README es para tu perfil de GitHub (repositorio `tu-usuario/tu-usuario`). Reemplaza los placeholders marcados como `TODO`.*

---

### 🧰 Stack

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/GitHub-121013?style=for-the-badge&logo=github&logoColor=white" height="25"/>
  &nbsp;
  <img src="https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white" height="25"/>
</p>

> **Lo que mejor manejo:** HTML, CSS, JavaScript.
> **Ahora practicando:** React, Tailwind, consumo de APIs REST, pruebas básicas con Jest y accesibilidad (WAI‑ARIA).

---

### 🚀 Proyectos (sample)

* **Weather Now** — App del clima con `fetch` y cache local.
  *Rol:* Front‑End · *Focus:* API, estados simples, responsive.
  **Demo:** `https://TODO-tu-dominio.dev/weather` · **Repo:** `https://github.com/TODO_USUARIO/weather-now`

* **TaskFlow** — To‑Do PWA con `localStorage` y atajos de teclado.
  *Rol:* Front‑End · *Focus:* UX, accesibilidad y performance.
  **Demo:** `https://TODO-tu-dominio.dev/taskflow` · **Repo:** `https://github.com/TODO_USUARIO/taskflow`

* **UI Components Kit** — Componentes accesibles (modales, tabs, dropdowns) sin dependencias.
  *Rol:* Front‑End · *Focus:* Semántica, ARIA y vanilla JS.
  **Demo:** `https://TODO-tu-dominio.dev/ui-kit` · **Repo:** `https://github.com/TODO_USUARIO/ui-components`

---

### 📊 Métricas

<p align="center">
  <!-- Reemplaza TODO_USUARIO por tu usuario real de GitHub -->
  <img src="https://github-readme-stats.vercel.app/api?username=TODO_USUARIO&theme=cobalt&show_icons=true&count_private=true" />
  <br/><br/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=TODO_USUARIO&theme=dark&hide_border=true" />
  <br/><br/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=TODO_USUARIO&layout=compact&theme=dark&hide_border=true" />
</p>

---

### 🧪 Mini‑demo (HTML+CSS+JS)

*Pega esto en `index.html` si quieres una tarjeta personal rápida con tema claro/oscuro:*

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Luana Flores – Front‑End</title>
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
    const prefersDark = matchMedia('(prefers-color-scheme: dark)').matches;
    const saved = localStorage.getItem(key);
    function apply(theme){
      if(theme === 'light'){ root.setAttribute('data-theme','light'); }
      else if(theme === 'dark'){ root.removeAttribute('data-theme'); }
      else { prefersDark ? root.removeAttribute('data-theme') : root.setAttribute('data-theme','light'); }
      document.getElementById('status').textContent = `Tema: ${theme || 'auto'}`;
    }
    apply(saved);
    document.getElementById('toggle').addEventListener('click', ()=>{
      const next = localStorage.getItem(key) === 'light' ? 'dark' : localStorage.getItem(key) === 'dark' ? '' : 'light';
      localStorage.setItem(key, next);
      apply(next);
    });
  </script>
</body>
</html>
```

---

### 🤝 Contacto

<p align="center">
  <!-- TODO: Actualiza los enlaces con tus perfiles reales -->
  <a href="https://www.linkedin.com/in/TODO_LINKEDIN" target="_blank">
    <img alt="LinkedIn" width="26" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" />
  </a>
  &nbsp;&nbsp;
  <a href="mailto:TODO_CORREO@ejemplo.com">
    <img alt="Email" width="26" src="https://cdn-icons-png.flaticon.com/512/561/561127.png" />
  </a>
  &nbsp;&nbsp;
  <a href="https://twitter.com/TODO_TWITTER" target="_blank">
    <img alt="Twitter/X" width="26" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/twitter/twitter-original.svg" />
  </a>
  &nbsp;&nbsp;
  <a href="https://www.instagram.com/TODO_INSTAGRAM/" target="_blank">
    <img alt="Instagram" width="26" src="https://github.com/SatYu26/SatYu26/blob/master/Assets/Instagram.svg" />
  </a>
</p>

---

### 📈 Contador de visitas

<p align="center">
  <img src="https://profile-counter.glitch.me/TODO_USUARIO/count.svg" />
</p>

---

### 🏆 Trofeos

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=TODO_USUARIO&theme=radical&margin-h=15&margin-w=5&no-bg=true" alt="TROPHY" />
</p>

---

### 🔖 Notas rápidas

* Español · Front‑End Junior · Ingeniería de Software con IA.
* Resalta habilidades: **HTML, CSS, JavaScript**.
* Incluye secciones listas para proyectos, métricas, trofeos y contacto.
* Reemplaza `TODO_USUARIO`, `TODO_LINKEDIN`, `TODO_CORREO`, `TODO_TWITTER`, `TODO_INSTAGRAM`.

---

*Última edición: 15/08/2025*

