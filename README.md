# CSS Day — Frontend Masters CSS Foundations Project

A compact, **fully responsive** multi‑page website built during the _Frontend Masters_ **CSS Foundations** workshop. The project showcases vanilla **HTML/CSS/JS**, modern layout techniques (Flexbox + Grid), and the **BEM** naming methodology.

> **Live demo**: open `index.html` in your browser or run a local dev server (see [Quick Start](#quick-start)).

---

## ✨ Features

- **Responsive design** — mobile‑first styles with `@media` breakpoints at 1000 px and 840 px.
- **Hamburger navigation** — JavaScript‑powered slide‑in menu for small screens.
- **Speakers page** — card grid built with `grid-template-columns`, collapsing gracefully to one column on mobile.
- **Semantic & accessible** markup (`<header>`, `<nav>`, `aria` labels).
- **CSS custom properties** (`--color‑primary`, `--color‑text‑on‑secondary`, …) for easy theming.
- **BEM** class naming (`block__element--modifier`) for predictable, maintainable styles.

---

## 🚀 Quick Start

```bash
# 1. Clone the repo
$ git clone https://github.com/panovark/fem-css-foundations
$ cd fem-css-foundations

# 2. Start a local dev server (choose one):

# Option A: VS Code Live Server extension
#   just right‑click index.html → “Open with Live Server”

# Option B: serve package (npm ≥ 9)
$ npx serve .

# Option C: Python 3 built‑in HTTP server
$ python -m http.server 8080
```

Then navigate to [http://localhost:8080](http://localhost:8080) (or the port Live Server prints).

---

## 🗂️ Project Structure

```
fem-css-foundations/
├── index.html          # Home page
├── speakers.html       # Speakers line‑up
├── index.js            # Mobile‑nav toggle logic
├── styles/
│   ├── base.css        # Tokens, resets, shared utilities
│   ├── index.css       # Home‑page specific styles
│   └── speakers.css    # Speakers page styles
├── fonts/              # Inter variable font
├── icons/              # SVG icons for UI
└── readme-images/      # Assets used in the course README
```

> **Tip:** Each stylesheet is split by page to keep bundles minimal; shared rules live in `styles/base.css`.

---

## 🛠️ Development Notes

### BEM Cheat‑Sheet

- **Block**: `.header`, `.nav`, `.card`
- **Element**: `.card__title`, `.nav__item`
- **Modifier**: `.menu--hide`, `.nav--visible`, `.card--featured`

```html
<!-- example -->
<button class="button button--primary">Save</button>
```

### Custom Breakpoints

```css
@media (max-width: 1000px) {
  /* tablet */
}
@media (max-width: 840px) {
  /* mobile */
}
```

### Scripts

There is **no build step**. All files are plain static assets so the site can be hosted on **GitHub Pages**, **Netlify Drop**, or any static host.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your‑feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push to your branch: `git push origin feature/your-feature`.
5. Open a Pull Request.

Please follow the existing code style (Prettier config included) and keep class names in BEM.

---

## 🙏 Credits

Built as part of the [Frontend Masters ](https://frontendmasters.com/courses/css-foundations/)[**CSS Foundations**](https://frontendmasters.com/courses/css-foundations/) course by Emma Bostian.
