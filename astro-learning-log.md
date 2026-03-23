# 🚀 My Astro Learning Log
> Goal: Build my own portfolio site from scratch and understand every part of it.

---

## 📌 Why I'm Learning This
- I've been using AI tools to build sites, but I want to understand the code myself
- So I can tell AI tools exactly what to customize, instead of guessing
- I want to build my own portfolio using the Astro framework

---

## 🗺️ My Learning Path
1. ✅ Understand what Astro is and why it's good for portfolios
2. ⬜ Set up the Astro project on my computer
3. ⬜ Understand the folder structure
4. ⬜ Create my first page
5. ⬜ Build a Layout (shared header/footer)
6. ⬜ Build reusable Components (cards, nav, hero section)
7. ⬜ Style the site with CSS
8. ⬜ Add my projects and about page
9. ⬜ Deploy the site online for free

---

## 📚 Concepts I've Learned

### What is Astro?
- A web framework made for **content-focused sites** (portfolios, blogs, docs)
- Ships **zero JavaScript by default** → super fast loading
- Uses `.astro` files: HTML + a little JavaScript at the top
- Files in `src/pages/` automatically become URLs on your site

### How Astro compares to other frameworks
| Framework | Best For | Difficulty |
|-----------|----------|------------|
| **Astro** | Portfolios, blogs, content sites | Beginner-friendly |
| **Next.js** | Full-stack apps, SaaS products | Intermediate |
| **React** | Complex interactive UIs | Intermediate |
| **Angular** | Enterprise apps | Advanced |

### Key Vocabulary
| Word | What it means |
|------|--------------|
| **Component** | A reusable piece of your UI (e.g. a card, a navbar) |
| **Layout** | A wrapper template shared across multiple pages |
| **Page** | A file in `src/pages/` that becomes a URL |
| **Static site** | A site built into plain HTML files — fast and free to host |
| **Props** | Data you pass into a component to customize it |

---

## 🛠️ Project Setup

### Commands I used
```bash
# Check Node.js is installed
node -v

# Create a new Astro project
npm create astro@latest

# Go into the project folder
cd my-portfolio

# Start the development server
npm run dev
```

### My project is located at:
`[fill this in after setup]`

---

## 📁 Folder Structure (What each folder does)

```
my-portfolio/
├── src/
│   ├── pages/          ← Each file here = a page on your site
│   │   └── index.astro ← This is your homepage (yourdomain.com/)
│   ├── components/     ← Reusable UI pieces (Navbar, Card, Footer)
│   ├── layouts/        ← Page templates shared across pages
│   └── styles/         ← CSS files for styling
├── public/             ← Images, fonts, favicons (stays as-is)
├── astro.config.mjs    ← Astro settings file
└── package.json        ← Project info + list of dependencies
```

---

## 🏗️ Pages I've Built

| Page | File | URL | Status |
|------|------|-----|--------|
| Home | `src/pages/index.astro` | `/` | ⬜ Not started |
| About | `src/pages/about.astro` | `/about` | ⬜ Not started |
| Projects | `src/pages/projects.astro` | `/projects` | ⬜ Not started |

---

## 🧩 Components I've Built

| Component | File | What it does | Status |
|-----------|------|--------------|--------|
| Navbar | `src/components/Navbar.astro` | Top navigation bar | ⬜ |
| Footer | `src/components/Footer.astro` | Bottom of every page | ⬜ |
| ProjectCard | `src/components/ProjectCard.astro` | Shows one project | ⬜ |
| Hero | `src/components/Hero.astro` | Big intro section | ⬜ |

---

## 💡 Things I Want to Remember

> Add notes here as you learn. For example:
> - "To change the background color of the hero, go to `src/components/Hero.astro` and find `background-color`"
> - "The layout file is in `src/layouts/BaseLayout.astro` — edit this to change the header on every page"

-

---

## 🤖 How to Talk to AI Tools Effectively

Once you understand your code, you can give AI tools very specific instructions:

**Instead of:** "Make it look better"
**Say:** "In `src/components/Hero.astro`, change the `h1` font size to 3rem and make the background a dark navy color (#0a0f1e)"

**Instead of:** "Add a projects section"
**Say:** "Create a new component at `src/components/ProjectCard.astro` that accepts props: `title`, `description`, and `imageUrl`, and displays them in a card with a border"

---

## 📅 Progress Log

| Date | What I did | Notes |
|------|-----------|-------|
| 2026-03-23 | Started learning Astro | Understood what Astro is, folder structure, key concepts |
| | | |

---

*Last updated: 2026-03-23*
