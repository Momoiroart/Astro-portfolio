my note that explain how i understand any command, progress of how to using
Astro framework


03/23/2026 : Initialize Astro project
		to initialize project you have to have node.js in your machine first handed or download it before you start making your project. 

# **Astro Structure:**
---
// 1. FRONTMATTER  — runs on the server, before the page loads
// This is where you: import other components, define variables, fetch data
// Users never see this section
---

<!-- 2. HTML — what actually shows up in the browser -->
<h1>Hello</h1>

<style>
  /* 3. CSS STYLE — controls how the HTML looks */
  /* Only affects THIS file, won't leak into other components */
  h1 { color: pink; }
</style>
```

The `---` fences are the dividing line between logic and display. Everything above the second `---` is instructions. Everything below is what the user sees.

---

**How Layout.astro and Welcome.astro connect**

Think of it like nesting boxes:
```
index.astro          ← the assembler (just connects things)
  └── Layout.astro   ← the outer frame (html, head, body, fonts)
        └── <slot /> ← the empty hole where content goes
              └── Welcome.astro  ← your actual content fills that hole
# **How to customize:**
**To change any text:** find the HTML section, locate the tag, change what's between the opening and closing tags.

astro

```astro
<!-- Before -->
<p id="tagline">I build web portfolios...</p>

<!-- After - just change the words -->
<p id="tagline">I create games and digital experiences.</p>
```

**To change a color:** find it in the `<style>` block, update the hex code. If it uses `var(--pink)`, change the variable at the top and it updates everywhere.

css

```css
/* Before */
--pink: #ff6b9d;

/* After */
--pink: #ff4466;
```

**To add a new skill tag:** find the `#tags` div in the HTML, copy one `<span>` and paste a new one.

astro

```astro
<span class="tag">Python</span>
<span class="tag">Discord Bots</span>   ← add this line
```

**To change a font size:** find the CSS rule for that element and update `font-size`.

css

```css
/* Before */
#name { font-size: clamp(2.5rem, 6vw, 4.5rem); }

/* After - make it bigger */
#name { font-size: clamp(3rem, 7vw, 5.5rem); }
```



# **Command:**
- node -v : use to verify version of your version of node.js in your machine, also use as to confirm that you had the node.js itself because you can get it version.
- npm : the tool that helps you install, manage, and run packages (ready-made code libraries) for your project
- node.js : the engine that runs JavaScript on your computer
- `npm create astro@latest`Creates a new Astro project
- `npm install`Installs all packages a project needs
- `npm run dev`Starts your local development server
- `npm run build`Builds your site into final HTML files
- - `<nav>` — a special HTML tag that means "this is a navigation bar". It's like `<div>` but tells the browser this is for navigation
- `<a href="/">` — a link. `href` is where it goes. `/` means the homepage
- `<ul>` — unordered list (no numbers, just dots by default — we'll remove the dots with CSS)
- `<li>` — list item, one entry inside the `<ul>`
