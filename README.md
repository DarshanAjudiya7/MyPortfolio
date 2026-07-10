# Darshan Ajudiya — Portfolio

A fast, accessible, single-page developer portfolio built with plain HTML, Tailwind CSS and vanilla JavaScript — no build step required.

**Live site:** https://porfolio-mu-orpin.vercel.app/

---

## ✨ Features

- **Dark / light mode** — toggles via `data-theme`, remembers your preference with `localStorage`, and respects your OS setting on first visit
- **Scrollspy navigation** — the active nav link updates automatically as you scroll
- **Scroll progress bar** — thin gradient bar at the top tracks reading progress
- **Animated reveals** — sections fade/slide in on scroll using `IntersectionObserver` (auto-disabled for `prefers-reduced-motion`)
- **Animated counters & skill bars** — numbers and progress bars animate into view once
- **Filterable project grid** — filter projects by `React`, `Node.js`, or `UI / Frontend`
- **Working contact form** — client-side validation, then opens the visitor's email client pre-filled via `mailto:` (no backend needed)
- **Copy-to-clipboard email** — one click, with a toast confirmation
- **Embedded resume viewer** — PDF resume previews inline, plus a direct download button
- **Fully responsive** — mobile menu, fluid type scale, and a marquee skills strip that pauses on hover
- **Accessible by default** — skip-to-content link, visible focus states, `aria-pressed`/`aria-expanded` on interactive controls

## 🛠 Tech stack

| Layer      | Choice                                    |
|------------|--------------------------------------------|
| Markup     | Semantic HTML5                             |
| Styling    | [Tailwind CSS](https://tailwindcss.com/) (CDN) + custom CSS variables for theming |
| Type       | [Sora](https://fonts.google.com/specimen/Sora) (display), [Inter](https://fonts.google.com/specimen/Inter) (body), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (code/labels) |
| Icons      | [Font Awesome 6](https://fontawesome.com/) |
| Behavior   | Vanilla JavaScript (`IntersectionObserver`, Clipboard API, no frameworks) |

No `npm install`, no bundler — open the HTML file and it runs.

## 📁 Project structure

```
.
├── index.html                     # Entire site (markup, styles, scripts)
├── Darshan_Ajudiya_Resume.pdf     # Downloadable / embedded resume
└── projects/
    ├── profile.jpeg               # About section portrait
    ├── project1.jpeg              # Budget Accounting System
    ├── project2.png               # Portfolio Website
    ├── project3.png               # VibeFy
    ├── project4.png               # AlgoArena — LeetCode Clone
    ├── project5.png               # Twitter Clone
    └── project6.png               # Traveloopl
```

> Keep image filenames and the `projects/` folder path in sync with the `src` attributes in `index.html` — nothing else needs to change.

## 🚀 Getting started

1. Clone or download this repository.
2. Make sure `Darshan_Ajudiya_Resume.pdf` and the `projects/` folder sit next to `index.html`.
3. Open `index.html` directly in a browser, or serve it locally:

   ```bash
   npx serve .
   # or
   python3 -m http.server 8080
   ```

4. Visit `http://localhost:8080` (or the port shown).

## 🌐 Deployment

Because this is a static site, it deploys anywhere for free:

- **Vercel** — `vercel deploy` (or connect the repo in the dashboard)
- **Netlify** — drag-and-drop the folder, or connect via Git
- **GitHub Pages** — push to a repo, enable Pages on the `main` branch

No environment variables or server-side code are required.

## 🎨 Customization

- **Colors / theme** — edit the CSS custom properties in the `:root` and `[data-theme="dark"]` blocks at the top of `index.html`.
- **Content** — all copy (About, Skills, Timeline, Projects, Blogs) lives directly in the corresponding `<section>` — no CMS or data file.
- **Skills marquee** — add or remove `.tech-icon` entries inside `#skills`; the track duplicates its content automatically for a seamless loop.
- **Projects** — duplicate a `.project-card` block, update the image, copy, tags (`data-tags`) and live-demo link.
- **Contact form** — currently opens a pre-filled `mailto:` link. Swap the `submit` handler for a service like Formspree, EmailJS, or a serverless function if you'd like it to send without opening a mail client.

## 📬 Contact

- Email: [darshanajudiya07@gmail.com](mailto:darshanajudiya07@gmail.com)
- GitHub: [@DarshanAjudiya7](https://github.com/DarshanAjudiya7)
- LinkedIn: [darshan-ajudiya](https://www.linkedin.com/in/darshan-ajudiya-a5b301310/)
- X (Twitter): [@AjudiyaDarshan7](https://x.com/AjudiyaDarshan7)

## 📄 License

This project is personal portfolio code. Feel free to reference the structure or techniques, but please don't republish the content or images as your own.