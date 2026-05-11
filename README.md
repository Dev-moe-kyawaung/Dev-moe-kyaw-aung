<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=220&section=header&text=Moe%20Kyaw%20Aung&fontSize=58&fontColor=63b3ed&animation=fadeIn&fontAlignY=38&desc=Bootstrap%205%20%2B%20Three.js%203D%20Premium%20Portfolio&descAlignY=60&descColor=b794f4" width="100%"/>

<br/>

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Visit_Portfolio-63b3ed?style=for-the-badge&labelColor=0a0d16)](https://dev-moe-kyawaung.github.io/Developer-moekyawaung-portfolio/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3.3-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com)
[![Three.js](https://img.shields.io/badge/Three.js-r128-white?style=for-the-badge&logo=threedotjs&logoColor=black)](https://threejs.org)
[![License](https://img.shields.io/badge/License-MIT-63b3ed?style=for-the-badge)](LICENSE)

<br/>

```
╔═══════════════════════════════════════════════════════════════╗
║  Bootstrap 5  •  Three.js r128  •  AOS  •  Bootstrap Icons   ║
║  3D Particles  •  Tilt Cards  •  Flip Certs  •  Skill Bars   ║
╚═══════════════════════════════════════════════════════════════╝
```

</div>

---

## 📋 Table of Contents

- [Live Demo](#-live-demo)
- [Features](#-features)
- [Tech Stack & Dependencies](#-tech-stack--dependencies)
- [File Structure](#-file-structure)
- [Getting Started](#-getting-started)
- [CDN Dependencies](#-cdn-dependencies)
- [Sections](#-sections)
- [Customization](#-customization)
- [Deploy to GitHub Pages](#-deploy-to-github-pages)
- [Browser Support](#-browser-support)
- [License](#-license)

---

## 🌐 Live Demo

> **URL:** [https://dev-moe-kyawaung.github.io/Developer-moekyawaung-portfolio/](https://dev-moe-kyawaung.github.io/Developer-moekyawaung-portfolio/)

---

## ✨ Features

### 🎮 3D Animations (Three.js)
| Feature | Description |
|---|---|
| 🔷 Floating Particles | 80 icosahedra meshes floating across the canvas |
| 🌀 Wireframe Toruses | 2 rotating torus rings for depth |
| 🖱️ Mouse Parallax | Camera moves with mouse for immersive 3D feel |
| 🃏 Profile Card Tilt | Real-time 3D tilt effect on hover (16° Y, 10° X) |
| 🔄 Cert Card Flip | CSS 3D perspective flip on hover — front/back |
| ⚡ Breathing Opacity | Particles fade in/out with sinusoidal animation |

### 🎨 UI & Design
| Feature | Description |
|---|---|
| 🖱️ Custom Cursor | Dot + lagging ring cursor with hover scale effects |
| 📜 Scroll Reveal | AOS library — staggered fade/zoom on scroll |
| 📊 Skill Bars | Animated progress bars triggered by IntersectionObserver |
| 🌈 Gradient Text | CSS `background-clip: text` gradient on headings |
| 💎 Glass Cards | `backdrop-filter: blur()` frosted glass effect |
| 📱 Responsive | Mobile-first Bootstrap grid, hamburger nav |
| 🎯 Active Nav | Navbar shrinks and shadows on scroll |

### 📐 Bootstrap 5 Components Used
- `navbar` + `navbar-collapse` (responsive hamburger)
- `container`, `row`, `col-*` grid system
- `d-flex`, `gap-*`, `justify-content-*` utilities
- `data-bs-theme="dark"` global dark mode
- `data-bs-toggle="collapse"` for mobile menu

---

## 🛠️ Tech Stack & Dependencies

### External Libraries (CDN — no install needed)

| Library | Version | Purpose | CDN |
|---|---|---|---|
| **Bootstrap CSS** | 5.3.3 | UI framework, grid, utilities | jsDelivr |
| **Bootstrap Icons** | 1.11.3 | Icon font (600+ icons) | jsDelivr |
| **Bootstrap JS** | 5.3.3 | Navbar collapse, interactive components | jsDelivr |
| **Three.js** | r128 | 3D WebGL background animations | cdnjs |
| **AOS** | 2.3.4 | Animate On Scroll library | unpkg |
| **Google Fonts** | — | Clash Display, Cabinet Grotesk, Instrument Serif | Google APIs |

### Zero Build Tools Required
```
No npm    ✓
No webpack ✓
No node   ✓
No build  ✓
Pure HTML/CSS/JS — open index.html directly
```

---

## 📁 File Structure

```
Developer-moekyawaung-portfolio/
│
├── index.html                    # ★ Main portfolio (ALL-IN-ONE)
├── README.md                     # This documentation
├── LICENSE                       # MIT License
├── .gitignore                    # Git ignore rules
│
├── assets/                       # (Optional) Local assets
│   ├── images/
│   │   ├── profile.jpg           # Your profile photo
│   │   ├── og-image.jpg          # Open Graph preview image (1200×630)
│   │   └── projects/
│   │       ├── pulsesync.png     # PulseSync screenshot
│   │       ├── azure-app.png     # PulseSync Azure screenshot
│   │       └── roadmap-app.png   # Roadmap App screenshot
│   └── resume/
│       └── moe-kyaw-aung-cv.pdf  # Downloadable resume/CV
│
└── .github/
    └── workflows/
        └── deploy.yml            # GitHub Actions auto-deploy
```

> **Note:** `index.html` is fully self-contained. The `assets/` folder is optional for adding real photos and PDF resume.

---

## 🚀 Getting Started

### Option 1 — Open Directly (Fastest)
```bash
# Clone the repo
git clone https://github.com/Dev-moe-kyawaung/Developer-moekyawaung-portfolio.git

cd Developer-moekyawaung-portfolio

# Open in browser — no server needed!
open index.html               # macOS
start index.html              # Windows
xdg-open index.html           # Linux
```

### Option 2 — Local Dev Server (Recommended)
```bash
# Python (built-in)
python3 -m http.server 8080
# Visit: http://localhost:8080

# OR Node.js (npx — no install)
npx serve .
# Visit: http://localhost:3000

# OR VS Code — install "Live Server" extension
# Right-click index.html → "Open with Live Server"
```

> ⚠️ **Why a server?** Three.js WebGL and some CSS features work best on a local server rather than file:// protocol.

---

## 📦 CDN Dependencies

All dependencies are loaded via CDN — no local files needed. Here are the exact URLs used in `index.html`:

### CSS (in `<head>`)
```html
<!-- 1. Bootstrap 5.3.3 CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>

<!-- 2. Bootstrap Icons 1.11.3 -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css" rel="stylesheet"/>

<!-- 3. Google Fonts — Clash Display + Cabinet Grotesk + Instrument Serif -->
<link href="https://fonts.googleapis.com/css2?family=Clash+Display:wght@400;500;600;700&family=Cabinet+Grotesk:wght@300;400;500;700;800;900&family=Instrument+Serif:ital@0;1&display=swap" rel="stylesheet"/>

<!-- 4. AOS (Animate On Scroll) 2.3.4 CSS -->
<link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet"/>
```

### JavaScript (before `</body>`)
```html
<!-- 5. Bootstrap 5.3.3 JS Bundle (includes Popper.js) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

<!-- 6. AOS 2.3.4 JS -->
<script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>

<!-- 7. Three.js r128 -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
```

### Google Fonts Used
| Font | Weights | Usage |
|---|---|---|
| **Clash Display** | 400, 500, 600, 700 | Headings, nav, buttons |
| **Cabinet Grotesk** | 300, 400, 500, 700, 800, 900 | Body text, descriptions |
| **Instrument Serif** | 400, 400 italic | Decorative stroke text |

---

## 🗂️ Sections

| # | Section | Description |
|---|---|---|
| 1 | **Navbar** | Fixed top, blur backdrop, responsive collapse |
| 2 | **Hero** | 3D bg canvas, profile tilt card, stats row |
| 3 | **About** | Bio text + 6 highlight cards |
| 4 | **Skills** | 3 skill cards with animated bars + 12 tech orbs |
| 5 | **Experience** | Vertical timeline with 3 career entries |
| 6 | **Projects** | Featured + 3 project cards with 3D hover |
| 7 | **Certifications** | 6 flip cards (front/back 3D) |
| 8 | **Contact** | Contact links + message form |
| 9 | **Footer** | Brand, copyright, social links |

---

## 🎨 Customization

### Change Colors
Edit CSS variables at the top of `<style>` in `index.html`:
```css
:root {
  --bg-deep:    #04050a;     /* Main background */
  --cyan:       #63b3ed;     /* Primary accent */
  --violet:     #b794f4;     /* Secondary accent */
  --rose:       #fc8181;     /* Tertiary accent */
  --gold:       #f6d860;     /* Warning/highlight */
}
```

### Change Personal Info
Search and replace in `index.html`:
```
"Moe Kyaw Aung"           → Your name
"moekyawaung@asia.com"    → Your email
"+95 988 9000 889"        → Your phone
"Dev-moe-kyawaung"        → Your GitHub username
"Tachileik, Myanmar"      → Your location
```

### Add Profile Photo
Replace the avatar letter `M` with an `<img>` tag:
```html
<!-- Find this in index.html: -->
<div class="avatar-inner-3d">M</div>

<!-- Replace with: -->
<img src="assets/images/profile.jpg"
     style="width:100%; height:100%; object-fit:cover; border-radius:50%;"
     alt="Moe Kyaw Aung">
```

### Add Resume Download
```html
<!-- Add this button in hero section: -->
<a href="assets/resume/moe-kyaw-aung-cv.pdf"
   download class="btn-outline-custom">
  <i class="bi bi-download"></i> Download CV
</a>
```

### Modify 3D Particles
Find the Three.js block and adjust:
```javascript
// Change particle count (default: 80)
for (let i = 0; i < 80; i++) { ... }

// Change particle color
color: 0x63b3ed   // cyan hex
color: 0xb794f4   // violet hex

// Change particle speed
vx: (Math.random() - 0.5) * 0.02,   // horizontal speed
vy: (Math.random() - 0.5) * 0.015,  // vertical speed
```

---

## 🚀 Deploy to GitHub Pages

### Method 1 — Manual Settings (Simple)
```
1. GitHub → Your Repo → Settings → Pages
2. Source: "Deploy from a branch"
3. Branch: main → / (root)
4. Save → Wait 2-3 minutes
5. Live at: https://dev-moe-kyawaung.github.io/Developer-moekyawaung-portfolio/
```

### Method 2 — GitHub Actions (Auto-deploy)
The included `.github/workflows/deploy.yml` auto-deploys on every `git push`:
```bash
git add .
git commit -m "🚀 Update portfolio"
git push origin main
# → Automatically deploys in ~60 seconds
```

### Method 3 — Netlify Drop (Instant)
```
1. Go to https://app.netlify.com/drop
2. Drag and drop the entire repo folder
3. Instant live URL — no account needed
```

---

## 🌍 Browser Support

| Browser | Support | Notes |
|---|---|---|
| Chrome 90+ | ✅ Full | Recommended |
| Firefox 88+ | ✅ Full | |
| Safari 14+ | ✅ Full | |
| Edge 90+ | ✅ Full | |
| Mobile Chrome | ✅ Full | Touch events |
| Mobile Safari | ✅ Full | iOS 14+ |
| IE 11 | ❌ No | Not supported |

> **WebGL Required:** Three.js 3D background needs WebGL support. All modern browsers support this. Falls back gracefully (canvas hidden) if unsupported.

---

## ⚡ Performance

| Metric | Value |
|---|---|
| Total file size | ~1 HTML file (~85KB) |
| External CSS CDN | Bootstrap + Icons + AOS + Fonts |
| External JS CDN | Bootstrap JS + Three.js + AOS |
| No build step | Pure HTML/CSS/JS |
| Lighthouse Score | 90+ (after adding profile image) |

---

## 📬 Contact

<div align="center">

| Channel | Details |
|---|---|
| 📧 Email | [moekyawaung@asia.com](mailto:moekyawaung@asia.com) |
| 📱 Phone | [+95 988 9000 889](tel:+959889000889) |
| 💻 GitHub | [@Dev-moe-kyawaung](https://github.com/Dev-moe-kyawaung) |
| 🌐 Portfolio | [Live Site](https://dev-moe-kyawaung.github.io/Developer-moekyawaung-portfolio/) |

</div>

---

## 📄 License

```
MIT License — © 2026 Moe Kyaw Aung
Free to use as portfolio template with attribution.
```

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=100&section=footer" width="100%"/>
</div>