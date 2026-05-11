# 📦 Dependencies & Requirements
# Bootstrap 3D Portfolio — Moe Kyaw Aung
# All dependencies are loaded via CDN (no npm/pip needed)
# ═══════════════════════════════════════════════════════

# ──────────────────────────────────────────
# CSS DEPENDENCIES
# ──────────────────────────────────────────

bootstrap-css==5.3.3
# Source : https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css
# Purpose: UI framework — grid, utilities, components, dark mode

bootstrap-icons==1.11.3
# Source : https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css
# Purpose: Icon font — envelope, github, phone, arrow-right, etc.

aos-css==2.3.4
# Source : https://unpkg.com/aos@2.3.4/dist/aos.css
# Purpose: Animate On Scroll — fade/zoom/slide transitions

google-fonts-clash-display==latest
# Source : https://fonts.googleapis.com/css2?family=Clash+Display:wght@400;500;600;700
# Purpose: Display font — headings, nav, buttons, hero title

google-fonts-cabinet-grotesk==latest
# Source : https://fonts.googleapis.com/css2?family=Cabinet+Grotesk:wght@300;400;500;700;800;900
# Purpose: Body font — descriptions, paragraphs, labels

google-fonts-instrument-serif==latest
# Source : https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1
# Purpose: Decorative serif — italic stroke text in headings

# ──────────────────────────────────────────
# JAVASCRIPT DEPENDENCIES
# ──────────────────────────────────────────

bootstrap-js==5.3.3
# Source : https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js
# Purpose: Navbar collapse, Popper.js included (bundle)
# Includes: Popper.js 2.x (bundled)

three-js==r128
# Source : https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js
# Purpose: WebGL 3D background — particles, toruses, lighting, camera
# Features used:
#   - THREE.WebGLRenderer
#   - THREE.Scene / Camera / PerspectiveCamera
#   - THREE.IcosahedronGeometry
#   - THREE.TorusGeometry
#   - THREE.MeshStandardMaterial
#   - THREE.MeshBasicMaterial
#   - THREE.Mesh
#   - THREE.AmbientLight
#   - THREE.PointLight

aos-js==2.3.4
# Source : https://unpkg.com/aos@2.3.4/dist/aos.js
# Purpose: Scroll-triggered animations
# Config : { once: true, duration: 750, easing: 'ease-out-cubic', offset: 60 }

# ──────────────────────────────────────────
# BROWSER APIS (Native — no library)
# ──────────────────────────────────────────

IntersectionObserver==native
# Used for: skill bar animation trigger on scroll
# MDN: https://developer.mozilla.org/en-US/docs/Web/API/IntersectionObserver

requestAnimationFrame==native
# Used for: cursor animation loop, Three.js render loop
# MDN: https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame

WebGL==native
# Used for: Three.js renderer
# Required: WebGL 1.0+ (all modern browsers)

CSS-backdrop-filter==native
# Used for: navbar blur, glass card effect
# Note: Requires -webkit-backdrop-filter for Safari

CSS-custom-properties==native
# Used for: design token variables (:root { --cyan: #63b3ed; })

# ──────────────────────────────────────────
# SYSTEM REQUIREMENTS
# ──────────────────────────────────────────

browser==Chrome>=90 OR Firefox>=88 OR Safari>=14 OR Edge>=90
webgl==required
javascript==enabled
internet==required-for-CDN-assets
node-js==NOT_REQUIRED
npm==NOT_REQUIRED
build-tool==NOT_REQUIRED

# ──────────────────────────────────────────
# OPTIONAL LOCAL ASSETS (not required)
# ──────────────────────────────────────────

# assets/images/profile.jpg       — Profile photo
# assets/images/og-image.jpg      — Open Graph image (1200x630)
# assets/images/projects/*.png    — Project screenshots
# assets/resume/*.pdf             — Downloadable CV/Resume