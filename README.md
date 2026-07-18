# Good News Community Education Centre — Website

Official website for **Good News CEC**, a primary school in Kahawa Wendani, Nairobi, Kenya.

Built with [Astro](https://astro.build) — fast, static, mobile-first.

---

## Tech Stack

- **Framework:** Astro (static site generation)
- **Styling:** Vanilla CSS with design tokens (no Tailwind, no frameworks)
- **Fonts:** Lexend + Source Sans 3 (Google Fonts)
- **Design:** Professional teal/blue palette, mobile-first, no glassmorphism

---

## Pages

| Route | Description |
|---|---|
| `/` | Home — Hero, Trust Bar, Features, Headteacher, CTA |
| `/about` | About Us — Mission, Vision, Core Values |
| `/admissions` | Admissions — Steps, Required Documents |
| `/contact` | Contact — Info, Map, Contact Form |

---

## Project Structure

```
squalid-spectrum/
├── public/
│   ├── images/
│   ├── styles/          # All CSS files (design tokens in global.css)
│   ├── logo.png
│   └── hero.png
├── src/
│   ├── components/      # Astro components per section
│   ├── layouts/
│   │   └── Layout.astro # Root layout with Navbar + Footer
│   └── pages/           # index, about, admissions, contact
├── astro.config.mjs
└── package.json
```

---

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server at localhost:4321
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

---

## Design Constraints

- No glassmorphism / no `backdrop-filter`
- No CSS frameworks — pure design tokens
- Mobile-first breakpoints: 375 → 640 → 768 → 1024 → 1200px
- Touch targets ≥ 44px on all interactive elements
- `prefers-reduced-motion` respected on all animations

---

## Deployment

Static output in `./dist/` — deploy to any static host (Netlify, Vercel, GitHub Pages, etc.).

---

## License

© Good News Community Education Centre. All rights reserved.
