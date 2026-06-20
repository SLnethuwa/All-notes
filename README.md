# උසස් සටහන් සහ උදව් — Blog

## 📁 Files
```
blog/
├── index.html              ← Homepage (post list)
└── posts/
    ├── n5-time-expressions.html
    ├── memory-vs-storage.html
    └── wifi-pentest-basics.html
```

## ✏️ Adding a new post (no coding knowledge needed)

1. Open any file inside `posts/` — copy it, rename it (e.g. `posts/my-new-topic.html`).
2. In the new file, change:
   - The `<title>` tag
   - The `<span class="stamp">` text (e.g. `日本語 · N5`, `ICT`, `Cyber`)
   - The `<h1>` and `<p class="meta">` (date)
   - Everything inside `<article>...</article>` — write your content using
     `<h2>` for section headings and `<p>` for paragraphs. Tables and the
     amber `<div class="note-box">` are already styled — just copy the
     pattern from an existing post.
3. Open `index.html`, copy one `<article class="card">...</article>` block
   near the top of `<main>`, and edit:
   - `data-tag` → `japanese`, `ict`, `cyber`, or `life` (controls the filter buttons)
   - The link `href="posts/your-file.html"` (two places)
   - The title, date, and excerpt text

That's it — no build step, no server needed.

## 🌍 Hosting it for free

**Easiest option — GitHub Pages:**
1. Create a free GitHub account at github.com
2. Create a new repository (e.g. `my-notes-blog`)
3. Upload the entire `blog` folder contents (index.html + posts/) to the repo
4. Go to repo **Settings → Pages → Source**, select the `main` branch, save
5. Your site goes live at `https://yourusername.github.io/my-notes-blog/`

**Alternative — Netlify (drag and drop, even easier):**
1. Go to app.netlify.com → sign up free
2. Drag the whole `blog` folder onto the "Deploy" area on the dashboard
3. Done — Netlify gives you a free `.netlify.app` URL instantly
4. You can later add a custom domain for free (Netlify) if you buy one separately

Both options are completely free for a static site like this, with no
expiration and no ads.

## 🎨 Design notes
- Colors: indigo header (#1B2A4A), warm paper background (#FAF6EE), amber accent (#C8762A)
- Fonts: Noto Serif Sinhala (headings), Noto Sans Sinhala (body), Space Mono (labels/meta) — loaded free from Google Fonts
- The "stamp" badge on each post is the signature visual element — like a library catalog card
