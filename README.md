Portfolio — Akshat Negi
Personal portfolio site for Akshat Negi — backend engineer working in Python, FastAPI, PostgreSQL, and message-queue-driven distributed systems.
Live site: https://akshatpsy.github.io/portfolio/
---
About
A single-page, single-file portfolio. No framework, no build step, no JavaScript — one `index.html` with inline CSS, which means it loads instantly, works with JS disabled, and can be hosted anywhere that serves static files.
The design follows a dark editorial layout on a 7-column grid: oversized display headline, numbered sections, and hairline borders instead of shadows.
Sections
#	Section	Contents
—	Hero	Positioning statement, availability status, primary links
01	Skills	Languages, Backend & APIs, Data & Storage, Systems & Reliability
02	Experience	Vosyn (Database Engineer Intern), Live Zone Design (Python Developer Intern)
03	Projects	Distributed Task Executor, Custom Language Interpreter, Adaptive Resource Provisioning, Memory Management Visualizer
04	Education	B.Tech CS, Graphic Era University + certifications
05	Contact	Email, phone, GitHub, LinkedIn
Tech
Semantic HTML5
Inline CSS — custom properties for theming, CSS Grid and Flexbox for layout
System font stack (no web-font requests); monospace for section labels
Responsive: 7-column desktop grid collapsing to a single column at 860px
Accessibility: WCAG AA contrast, visible keyboard focus, `prefers-reduced-motion` respected
Structure
```
.
├── index.html     # Entire site — markup + inline styles
├── .nojekyll      # Tells GitHub Pages to skip Jekyll processing
└── README.md
```
Run locally
Open the file directly:
```bash
open index.html        # macOS
start index.html       # Windows
```
Or serve it over HTTP:
```bash
python3 -m http.server 8000
# visit http://localhost:8000
```
Deploy
GitHub Pages (current setup)
Push to the `main` branch
Settings → Pages → Deploy from a branch
Branch `main`, folder `/ (root)` → Save
Any push to `main` redeploys automatically in about a minute.
Alternatives — the site is fully static, so it drops into Netlify, Vercel, or Cloudflare Pages with no build command and `/` as the output directory.
Customizing
Colors and fonts are CSS custom properties defined in the `:root` block at the top of `index.html`:
```css
--canvas:  #0E0E0E;   /* page background */
--text:    #FFFFFF;   /* primary text   */
--muted:   rgba(255,255,255,.62);
--accent:  #5E9FE8;   /* links, bullets, role labels */
```
Change a value once and it updates everywhere. Content lives in plain HTML — edit the text between the `<section>` tags to update skills, roles, or projects.
Contact
Email: akshatnegi322@gmail.com
GitHub: @Akshatpsy
LinkedIn: akshat-negi
Location: Dehradun, India · open to remote
---
© 2026 Akshat Negi. Content and design are personal work; feel free to read the source for reference.
