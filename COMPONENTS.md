# 🧩 Components Reference
> Bootstrap 3D Portfolio — All UI components documented

---

## 📐 Layout Components

### 1. Fixed Navbar
```
Location : index.html → <nav id="mainNav">
Bootstrap : .navbar .navbar-expand-lg .fixed-top
Features  :
  - backdrop-filter blur on scroll (.scrolled class)
  - Brand logo with gradient text
  - Responsive collapse (hamburger on mobile)
  - Smooth scroll to sections on link click
  - Hire Me CTA button (hidden on mobile)
Customise : Change nav-link hrefs to match your section IDs
```

### 2. Three.js 3D Canvas
```
Location : index.html → <canvas id="bg-canvas">
Library  : Three.js r128
Features :
  - 80 floating IcosahedronGeometry particles
  - 2 wireframe TorusGeometry rings
  - AmbientLight (cyan) + 2x PointLight
  - Mouse parallax — camera follows cursor
  - Particles wrap around edges (boundary loop)
  - Opacity breathing via Math.sin()
Customise :
  - Particle count  → change `80` in the for loop
  - Colors          → change hex values (0x63b3ed)
  - Speed           → adjust vx/vy userData values
  - Particle shape  → swap IcosahedronGeometry for others
```

---

## 🏠 Hero Section

### 3. Hero Badge (Status Indicator)
```
Location : #hero → .hero-badge
Features : Pulsing green dot + "Available for Opportunities" text
CSS      : animation: blink 1.8s ease infinite
Customise: Change text to "Open to Work", "Freelancing", etc.
```

### 4. Hero Title
```
Location : #hero → h1.hero-title
Fonts    : Clash Display (normal) + Instrument Serif (italic stroke)
Effects  :
  - .gradient-text  → background-clip: text gradient
  - .italic-serif   → transparent with -webkit-text-stroke
Customise: Edit the name text directly
```

### 5. Profile 3D Tilt Card
```
Location : #hero → #tiltCard
Features :
  - Mouse-move 3D tilt (perspective 800px)
  - rotateY(16deg) rotateX(10deg) max
  - Floating avatar animation (float-avatar keyframe)
  - Top gradient bar (3px)
  - Stats grid (3 columns)
  - Tech pills (.pill-cyan / .pill-violet / .pill-rose / .pill-gold)
  - Status pulse dot (.status-pulse animation)
JS       : mousemove event on #tiltCard element
Customise: Edit stat values, tech pills, location text
```

### 6. Quick Stats Row
```
Location : #hero → .row below hero-desc
Features : 3 stats with colored left border
Colors   : cyan (Years) | violet (Repos) | rose (CI/CD %)
Customise: Edit the numbers and labels directly in HTML
```

---

## 👤 About Section

### 7. Highlight Cards (6 cards)
```
Location : #about → .about-highlight-card
Bootstrap: col-sm-6 grid
Features :
  - Icon box with color variants (.hl-icon-cyan/violet/rose/gold)
  - Hover: translateY(-3px) + box-shadow
  - AOS: zoom-in with staggered delay (0, 80, 160, 240, 320, 400ms)
Customise: Change emoji, title, description per card
```

---

## 💡 Skills Section

### 8. Skill 3D Cards (3 cards)
```
Location : #skills → .skill-3d-card
Features :
  - Hover: perspective(800px) rotateX(3deg) translateY(-5px)
  - Animated progress bars (.bar-progress)
  - IntersectionObserver triggers animation at 25% visibility
  - Gradient fill: cyan → violet
  - Glow box-shadow on bars
JS       : barObs IntersectionObserver, data-w attribute for %
Customise: Edit skill names and data-w="97" percentage values
```

### 9. Tech Orb Grid (12 orbs)
```
Location : #skills → .tech-orb-grid
Bootstrap: CSS grid (4 columns)
Features :
  - Hover: translateY(-4px) scale(1.03)
  - Cyan border glow on hover
Customise: Change emoji icons and tech names
```

---

## 💼 Experience Section

### 10. Vertical Timeline
```
Location : #experience → .timeline-wrap
Features :
  - ::before pseudo-element as vertical gradient line
  - Dots (.timeline-dot) with glow box-shadow
  - Hover: dot scales 1.3x + background fills
  - Card hover: translateX(6px) + shadow
  - Achievement list with ▸ cyan arrow prefix
  - Color-coded dates (cyan/violet/rose per entry)
Customise: Add/remove .timeline-item blocks
```

---

## 🚀 Projects Section

### 11. Featured Project Card
```
Location : #projects → .project-card-3d (first, col-12)
Features :
  - Full-width featured layout
  - .project-shine overlay (white gradient)
  - Hover: perspective(1000px) rotateY(-3deg) rotateX(3deg) translateZ(10px)
  - Metrics chips row (3 chips)
  - Stack mini pills
Customise: Edit metrics values and stack badges
```

### 12. Regular Project Cards (3 cards)
```
Location : #projects → .project-card-3d (col-lg-4)
Features :
  - Individual color top bars per project
  - Unique icon-wrap background colors
  - GitHub link button (.project-link-btn)
  - Star badge pill
Customise: Change project title, description, stack, links
```

---

## 🏆 Certifications Section

### 13. Flip Cards (6 cards)
```
Location : #certifications → .cert-flip-card
Features :
  - CSS 3D perspective flip on hover (rotateY 180deg)
  - .cert-front → shows icon + title + institution
  - .cert-back  → shows gradient bg + description
  - backface-visibility: hidden for clean flip
  - Transition: 0.6s cubic-bezier(0.4,0,0.2,1)
  - AOS: zoom-in staggered (0, 60, 120, 180, 240, 300ms)
Customise: Edit cert-title-f, cert-inst, cert-back-text per card
```

---

## 📬 Contact Section

### 14. Contact Link Rows
```
Location : #contact → .contact-row
Features :
  - Hover: translateX(5px) + cyan border + bg tint
  - Icon box with color per channel
  - Right arrow indicator
  - <a> tags — email, tel, github, linkedin
Customise: Update href values with real contact info
```

### 15. Message Form
```
Location : #contact → .contact-card form area
Bootstrap: .row .col-sm-6 grid for name/email
Features :
  - .form-control-custom — dark styled inputs
  - Focus: cyan border + subtle glow
  - Submit button: gradient bg + hover lift
  - JS onClick: changes text to "Message Sent!" temporarily
Note     : Form is frontend-only. To make it functional,
           integrate Formspree: https://formspree.io
           or EmailJS: https://www.emailjs.com
```

---

## 🔢 Global Utilities

### Custom Cursor
```
Elements : #cursor-dot + #cursor-ring
JS       : requestAnimationFrame loop with lerp (0.13 factor)
Hover    : scale(2.5) dot + scale(1.6) ring + violet border
```

### AOS Scroll Animations
```
Library  : AOS 2.3.4
Config   : { once:true, duration:750, easing:'ease-out-cubic', offset:60 }
Types used: fade-right, fade-left, fade-up, zoom-in
Delay    : data-aos-delay="0/100/200" for stagger
```

### Navbar Scroll Effect
```
JS       : scroll event listener
Trigger  : window.scrollY > 60
Effect   : adds .scrolled class → padding shrinks + shadow
```

---

## 🎨 CSS Design Tokens

```css
/* Edit these in :root {} to retheme the entire site */
--bg-deep:     #04050a    /* Page background */
--bg-card:     #0a0d16    /* Card background */
--bg-glass:    rgba(10,13,22,0.7)  /* Glass backdrop */
--border:      rgba(255,255,255,0.06)
--border-glow: rgba(99,179,237,0.25)
--cyan:        #63b3ed    /* Primary accent */
--cyan-bright: #90cdf4    /* Hover state */
--violet:      #b794f4    /* Secondary accent */
--rose:        #fc8181    /* Tertiary accent */
--gold:        #f6d860    /* Warning/highlight */
--text:        #e2e8f0    /* Main text */
--text-muted:  #718096    /* Muted text */
--text-dim:    #a0aec0    /* Dimmed text */
--font-display: 'Clash Display'
--font-body:    'Cabinet Grotesk'
--font-serif:   'Instrument Serif'
--grad-main:   linear-gradient(135deg, #63b3ed 0%, #b794f4 100%)
--shadow-glow: 0 0 40px rgba(99,179,237,0.12), 0 20px 60px rgba(0,0,0,0.5)
```