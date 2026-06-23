# ItisAnannya.github.io
Created a personal portfolio about by self using HTML, CSS.

---

## Original HTML (as pasted)

```html
<!DOCTYPE html>
<html>
<head>
    <title>Anannya's Portfolio</title>
</head>
<body>

    <h1>Anannya Sharma</h1>
    <h3>BCA Student | AI/ML Enthusiast</h3>

    <hr>

    <h2>Introduction</h2>
    <p>
        Hi ! My name is Anannya Sharma. I am currently pursuing BCA.
        I am passionate about AI/ ML ,space research, and Full-Stack Development.
        I really take interest in learning new technologies and then creating some projects take can solve real - world problems .
        My current aim is to become to perform best as a full - stack development intern and contribute to innovative technology solutions.
    </p>

    <h2>Education</h2>
    <p><b>Degree:</b>BCA - No stream ( 1st Year)</p>
    <p><b>Status:</b> Currently Pursuing</p>

    <h2>Technical Skills</h2>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>Java</li>
        <li>Python</li>
        <li>DBMS(SQL)</li>
        <li>Artificial Intelligence / Machine Learning</li>
    </ul>

    <h2>On - Going Projects</h2>

    <h3>1. Hand - Tracking Interactive Website </h3>
    <p>
    Building a full website using Next.js inside VS Code that allows users to interact with web elements using a
    webcam.
    Integrating Google's MediaPipe framework to track real-time finger movements, pinches, and hand gestures.
    Writing clean JavaScript algorithms to turn hand coordinates into smooth onscreen video controls and page
     scrolling.
      </p>
    <p>
        <b>Technologies Used:</b> TensorFlow.js , Next.js, JavaScript ,Three.js , WebXR API , WebRTC
    </p>
    <h3>2. TO_DO_LIST</h3>
    <p>
        Currently developing a 'To-Do List' application using Python for backend logic and HTML and CSS for an
intuitive user interface, designed to help users efficiently manage their daily tasks.
    </p>
    <p>
        <b>Technologies Used:</b> Java Script, HTML, CSS
    </p>

    <h3>3. Portfolio Website</h3>
    <p>
        Created a personal portfolio website to showcase educational background,
        technical skills, projects, and contact information.
    </p>
    <p>
        <b>Technologies Used:</b> HTML, CSS
    </p>

    <h2>Internship Experience</h2>
    <p>
        Participating in internship activities involving frontend development,
        backend concepts, UI/UX design, project documentation, and  in short full - stack  development practices.
    </p>

    <h2>Strengths</h2>
    <ul>
        <li>Strong Technical Foundation</li>
        <li>Problem‑Solving & Innovation</li>
        <li>Full Stack Exposure</li>
        <li>AI/ML Training</li>
        <li>Hands‑On Project Experience</li>
    </ul>

    <h2>Hobbies</h2>
    <ul>
        <li>Learning New Technologies</li>
        <li>Drawing </li>
        <li>Listening to Music</li>
        <li>Cooking</li>
    </ul>

    <h2>Contact Me</h2>
    <p><b>Name:</b> Anannya Sharma</p>
    <p><b>Email:</b> as09lkoh@example.com</p>
    <p><b>Phone:</b> +91 XXXXXXXXXX</p>
    <p><b>LinkedIn:</b> linkedin.com/in//anannya-sharma-2ab335396</p>
    <p><b>GitHub:</b> github.com/https:/ItisAnannya</p>

    <hr>

    </body>
    </html>
```

---

## This conversation (added here)

Below is the assistant's short answer and the suggested improvements I provided when you asked whether the HTML would run and why colours weren't showing in the README.

Short answer: Yes — the HTML will run in a browser, but GitHub's README rendering strips most CSS and style attributes, so you won't see colored headings there. To get colors "like usual" add CSS and open the file as a normal HTML page (or add an index.html to your ItisAnannya.github.io repo so GitHub Pages serves it).

What I suggested and why
- Explained that README.md rendering on GitHub sanitizes HTML/CSS, removing colors.
- Provided a cleaned-up, styled index.html you can publish with GitHub Pages so the colors and layout appear correctly.

### Suggested index.html (save this to the repository root to publish via GitHub Pages)

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Anannya Sharma — Portfolio</title>
  <style>
    :root{
      --accent: #1e7e34; /* green */
      --bg: #f7f9fb;
      --card: #ffffff;
      --muted: #555;
      --maxw: 900px;
    }
    body{
      font-family: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg, var(--bg), #eef4f1);
      color:#222;
      margin:0;
      padding:32px;
      display:flex;
      justify-content:center;
    }
    .container{
      width:100%;
      max-width:var(--maxw);
      background:var(--card);
      padding:28px;
      border-radius:12px;
      box-shadow:0 8px 30px rgba(18, 35, 30, 0.08);
    }
    header h1{
      margin:0;
      color:var(--accent);
      letter-spacing:0.4px;
    }
    header h3{
      margin:6px 0 18px;
      color:#222;
      font-weight:500;
    }
    hr{ border:0; height:1px; background:#eee; margin:18px 0; }
    h2{ color:var(--accent); margin-top:20px; }
    h3.project{ color:#0b6623; margin-bottom:6px; }
    p, li{ line-height:1.55; color:var(--muted); }
    ul{ padding-left:1.2rem; }
    .skills li{ display:inline-block; background:#f0fff4; color:var(--accent); margin:6px 8px 6px 0; padding:6px 10px; border-radius:8px; font-weight:600; }
    .contact a{ color:var(--accent); text-decoration:none; }
    footer{ margin-top:20px; font-size:0.9rem; color:#888; }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Anannya Sharma</h1>
      <h3>BCA Student | AI/ML Enthusiast</h3>
    </header>

    <hr/>

    <section>
      <h2>Introduction</h2>
      <p>
        Hi! I'm Anannya Sharma, currently pursuing BCA. I'm passionate about AI/ML, space research, and full‑stack development.
        I enjoy learning new technologies and building projects that solve real‑world problems. My current aim is to work as a
        full‑stack intern and contribute to innovative solutions.
      </p>
    </section>

    <section>
      <h2>Education</h2>
      <p><strong>Degree:</strong> BCA (1st Year)</p>
      <p><strong>Status:</strong> Currently Pursuing</p>
    </section>

    <section>
      <h2>Technical Skills</h2>
      <ul class="skills">
        <li>HTML</li>
        <li>CSS</li>
        <li>Java</li>
        <li>Python</li>
        <li>DBMS (SQL)</li>
        <li>AI / ML</li>
      </ul>
    </section>

    <section>
      <h2>On‑Going Projects</h2>

      <h3 class="project">1. Hand‑Tracking Interactive Website</h3>
      <p>
        Building an interactive website (Next.js) that uses the webcam to control UI with hand gestures (MediaPipe/TensorFlow.js).
        Includes smooth gesture → UI mappings and WebRTC for webcam access.
      </p>
      <p><strong>Technologies:</strong> TensorFlow.js, Next.js, JavaScript, Three.js, WebXR, WebRTC</p>

      <h3 class="project">2. To‑Do List</h3>
      <p>
        Developing a To‑Do application with Python backend and an intuitive HTML/CSS frontend for task management.
      </p>
      <p><strong>Technologies:</strong> Python, JavaScript, HTML, CSS</p>

      <h3 class="project">3. Portfolio Website</h3>
      <p>
        A personal website showcasing background, skills, projects, and contact information.
      </p>
      <p><strong>Technologies:</strong> HTML, CSS</p>
    </section>

    <section>
      <h2>Internship Experience</h2>
      <p>
        Involved in frontend development, backend concepts, UI/UX design, and project documentation — gaining full‑stack exposure.
      </p>
    </section>

    <section>
      <h2>Strengths</h2>
      <ul>
        <li>Strong technical foundation</li>
        <li>Problem solving & innovation</li>
        <li>Full‑stack exposure</li>
        <li>AI/ML training</li>
        <li>Hands‑on project experience</li>
      </ul>
    </section>

    <section>
      <h2>Hobbies</h2>
      <ul>
        <li>Learning new technologies</li>
        <li>Drawing</li>
        <li>Listening to music</li>
        <li>Cooking</li>
      </ul>
    </section>

    <section class="contact">
      <h2>Contact</h2>
      <p><strong>Email:</strong> <a href="mailto:as09lkoh@example.com">as09lkoh@example.com</a></p>
      <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/anannya-sharma-2ab335396" target="_blank" rel="noopener">anannya-sharma-2ab335396</a></p>
      <p><strong>GitHub:</strong> <a href="https://github.com/ItisAnannya" target="_blank" rel="noopener">ItisAnannya</a></p>
    </section>

    <footer>
      <p>Designed with ❤️ — feel free to edit and style further.</p>
    </footer>
  </div>
</body>
</html>
```

---

### How to preview or publish
- To preview locally: save the above index.html and open it in your browser (or run a simple server: `python -m http.server`).
- To publish on GitHub Pages: put `index.html` in the root of this repository (ItisAnannya/ItisAnannya.github.io) on the default branch — GitHub Pages will serve it at https://ItisAnannya.github.io.

---

If you want, I can also add the index.html file to your repository now so the live site shows the styled version. Tell me if I should create `index.html` on the default branch.