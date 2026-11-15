# Role & Objective
You are an elite creative frontend engineer specializing in award-winning, fluid, highly animated creative portfolios (Awwwards/FWA standard). Build a production-ready, highly animated portfolio website for thumbnail designer "YashGFX" using HTML, Tailwind CSS, GSAP (with ScrollTrigger), and Three.js / Canvas.

---

## 1. Strict Color Palette & Layout Architecture
Adhere strictly to this designated Primary Color Palette across all components:

- **Primary Accent:**
  - Name: Vermilion Red / Crimson
  - Hex: `#D24939` | RGB: `rgb(210, 73, 57)`
  - Usage: Continuous central vertical stripe/pillar, accent highlights, bold CTAs, aive/hover states, and glowing edge accenct
- **Background:**
  - Name: Warm Concrete Grey
  - Hex: `#D3D3D3` | RGB: `rgb(211, 211, 211)`
  - Usage: Main canvas background and light negative space flanking the central column.
- **Typography & Outlines:**
  - Name: Ink Black
  - Hex: `#131313` | RGB: `rgb(19, 19, 19)`
  - Usage: Heavy display typography, primary headings, text outlines, borders, and structural dividers.

### Layout Mechanics
- **Central Vertical Stripe:** Implement a continuous vertical column in `#D24939` centered horizontally, running without interruption through the full scroll height of the page.
- **Flanking Canvas:** Keep the outer areas styled in `#D3D3D3` with sharp `#131313` line borders separating sections.
- **Scroll Physics:** Integrate Lenis Smooth Scroll globally for inertia and weighted deceleration.

---

## 2. Page Structure & Interactive Modules

### Phase 1: Preloader (MangoFX Style Match)
- **Overlay:** Fullscreen fixed curtain (`fixed inset-0 z-50 bg-[#131313] flex flex-col items-center justify-center`).
- **Typography:** Display text **"Yash.GFX"** rendered dead-center in bold `#D3D3D3` with `#D24939` accenting, masked via clip-path for an upward slide reveal.
- **Counter:** High-speed numeric percentage (`00%` -> `100%`) in a tracked monospace font using GSAP ticker logic.
- **Exit Sequence:** At `100%`, "Yash.GFX" slides up through its mask while the background splits or vertically wipes away to smoothly expose the hero section.

### Phase 2: Navigation Bar (Image 1 / MangoFX Style)
- **Layout:** Floating pill navbar centered at the top (`backdrop-blur-md bg-[#131313]/90 border border-[#D3D3D3]/20`).
- **Elements:**
  - Left: "YashGFX" minimal wordmark.
  - Center/Right: Nav items ("Work", "Services", "About", "Contact") with magnetic cursor pull and kinetic `#D24939` underline sweeps on hover.
  - CTA Button: Pill-shaped button styled in `#D24939` with `#131313` text and inverse hover state.

### Phase 3: Hero Section (Image 2 Inspired)
- **Central Element (1/3 of the Homepage):**
  - A persistent, kinetic 3D typographic element displaying "YashGFX" rotating continuously around its Y-axis inside the central `#D24939` column.
  - Implement using Three.js or GSAP 3D CSS transforms with dynamic perspective and mouse-drag acceleration.
- **Hero Typography:** Heavy Ink Black (`#131313`) display typography layered behind and in front of the 3D rotating text.

### Phase 4: Thumbnail Showcase Grid (Image 3 / MangoFX Style)
- **Presentation:** High-impact showcase displaying YouTube thumbnail designs.
- **Interactions:**
  - Staggered multi-column grid with 3D tilt-on-hover physics tracking mouse coordinates.
  - Hover states: Micro-zoom, glare shader reflections, and floating metric pills (CTR%, View counts, Creator handles).
  - Lightbox / modal zoom on thumbnail click with morph layout animations.

### Phase 5: Metrics & Credibility Ticker (Image 4 / KBashed Style)
- **Content:** Large credibility statistics (e.g., "100M+ Views", "500+ Thumbnails", "Top 1% CTR").
- **Motion:**
  - GSAP ScrollTrigger numeric counters scrubbing upward on scroll.
  - Dual infinite marquee text bands moving in opposite directions across the `#D24939` stripe using `#131313` typography.

### Phase 6: Workflow & Creative Vault (Image 5 / KBashed Style)
- **Layout:** Interactive pinned horizontal scroll section or tabbed accordion detailing the thumbnail creation lifecycle (Strategy -> 3D Composition -> Retouching -> CTR Testing).
- **Interactive Component:** Before/After thumbnail comparison slider with smooth mouse-drag tracking.

### Phase 7: Footer & Social Connect Grid (Image 6 / MangoFX Style)
- **Headline:** Giant display text: "READY TO DOMINATE THE ALGORITHM?" in `#131313`.
- **Social Grid:**
  - Interactive magnetic cards for Twitter/X, Discord, YouTube, Behance, and Instagram.
  - Hover states: Button background dynamically fills with `#D24939` while text shifts to `#D3D3D3`.
  - Include live local time indicator and a smooth "Scroll to Top" kinetic button.

---

## 3. Technical Implementation
- Deliver functional, production-ready code (HTML5, Tailwind CSS via CDN, GSAP 3.x with ScrollTrigger, Lenis, and Three.js).
- Ensure complete mobile responsiveness, accessible contrasts, and GPU-accelerated transforms (`will-change: transform`).
- Use accessible CDN image placeholders for all thumbnail slots so they can easily be replaced with local assets.