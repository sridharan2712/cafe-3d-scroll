<div align="center">

# 🚢 NAVIS — Luxury Cruises

### Precision Engineering. Global Maritime Standards. Building the Future of the Seas.

[![Next.js](https://img.shields.io/badge/Next.js-16.2.9-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2.4-61DAFB?style=for-the-badge&logo=react)](https://react.dev/)
[![Three.js](https://img.shields.io/badge/Three.js-0.185-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![GSAP](https://img.shields.io/badge/GSAP-3.15-88CE02?style=for-the-badge&logo=greensock)](https://gsap.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)

An immersive, scroll-driven luxury cruise showcase featuring frame-by-frame cinematic animations, 3D WebGL ocean scenes, interactive bento grids, and premium dark-themed UI — built with Next.js 16, React Three Fiber, and GSAP ScrollTrigger.

</div>

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Project Description](#-project-description)
- [Objectives](#-objectives)
- [Key Features](#-key-features)
- [Technologies Used](#-technologies-used)
- [Tools and Frameworks](#-tools-and-frameworks)
- [Project Architecture](#-project-architecture)
- [Folder Structure](#-folder-structure)
- [Installation and Setup](#-installation-and-setup)
- [Prerequisites](#-prerequisites)
- [How to Run the Project](#-how-to-run-the-project)
- [Usage Instructions](#-usage-instructions)
- [Future Enhancements](#-future-enhancements)
- [Contributing Guidelines](#-contributing-guidelines)

---

## 🌊 Project Overview

**NAVIS** is a high-end, single-page marketing website for a luxury cruise line. It pushes the boundaries of modern web experiences by combining scroll-driven frame-by-frame video animations (900 sequential image frames), real-time 3D WebGL ocean rendering, CSS-based 3D perspective effects, and micro-interaction design — all within a premium dark navy aesthetic.

The site is built as a fully static Next.js application with no backend, no API calls, and no authentication — making it a pure front-end showcase of advanced web animation and interaction techniques.

---

## 📝 Project Description

NAVIS is designed as an immersive digital experience that communicates the luxury, craftsmanship, and elegance of a premium cruise line. Rather than relying on traditional static layouts, the website uses cinematic scroll-driven animations where each scroll movement advances a frame sequence — similar to how Apple's product pages work.

The website features multiple scroll-animated sections that tell the story of NAVIS — from ship engineering and construction to onboard dining, nightlife, and lifestyle experiences. Interactive elements include 3D mouse-tracking card tilts, expanding hover galleries, bento grid layouts, and a real-time Three.js ocean wave simulation with floating particle stars.

The UI follows a dark navy theme (`#0a0e1a`) with blue accents (`#2563eb`), frosted glassmorphism effects, a film grain texture overlay, and refined typography pairing Inter (sans-serif) with Playfair Display (serif).

---

## 🎯 Objectives

- **Immersive Storytelling** — Use scroll-driven animations to narrate the NAVIS brand story through cinematic frame sequences
- **Premium Visual Identity** — Deliver a luxury-tier dark-themed UI with glassmorphism, film grain, and refined typography
- **Advanced Web Animations** — Demonstrate GSAP ScrollTrigger, CSS 3D transforms, and WebGL in a production-quality website
- **Interactive User Experience** — Engage users with 3D mouse-tracking cards, expanding galleries, and hover micro-interactions
- **Performance at Scale** — Efficiently preload and render 900+ sequential animation frames without blocking the main thread

---

## ✨ Key Features

### 🎬 Scroll-Driven Frame Animation
- Three independent scroll-animated sections, each powered by **300 preloaded JPEG frames**
- GSAP ScrollTrigger scrubs through frames based on scroll position with smooth interpolation
- Story text panels dynamically appear and disappear at specific frame ranges
- Full-screen sticky canvas with cover-fit rendering

### 🌊 3D WebGL Ocean Scene
- Real-time animated ocean waves using Three.js vertex displacement (sine-wave animation)
- Blue wireframe grid overlay on the wave surface
- 600 floating particle stars using `@react-three/drei` Points system
- Rotating glowing torus ring
- Multi-point lighting setup (ambient + directional + point lights)

### 🃏 Interactive 3D Cards
- Mouse-tracking 3D tilt effect (±14° to ±18° rotateX/rotateY) with CSS `perspective` and `preserve-3d`
- Radial gradient shine layer that follows the cursor in real-time
- Depth layers using `translateZ` for parallax-within-card effect
- Elastic snap-back animation on mouse leave

### 📐 Bento Grid Layouts
- Nightlife section: 4-column × 3-row asymmetric bento grid with 8 cards of varying spans
- Pool section: Asymmetric grid with a large hero image spanning 2 rows
- Hover effects: image zoom, gradient overlay, label animation, description reveal

### 🎨 Premium UI Design
- Dark navy theme with blue accent color palette
- Frosted glassmorphism navigation bar (`backdrop-filter: blur`)
- SVG noise-based film grain texture overlay with stepping animation
- Custom ultra-thin scrollbar (3px, blue on navy)
- Infinite horizontal ticker marquee with cruise features

### 🎭 Preloader
- Full-screen branded loading screen with NAVIS wordmark
- Shimmer gradient animation on the logo
- Animated progress bar with blue gradient fill
- Smooth fade-out transition after loading completes

### 🍽️ Dining Marquee Gallery
- CSS-animated continuous horizontal scroll of food photography
- 8 images duplicated for seamless infinite loop (36s cycle)
- Rounded cards with hover zoom effect

### 🔤 Typography System
- **Inter** (400–900 weights) for UI text, labels, and body copy
- **Playfair Display** (700, italic) for editorial headings and accent text
- Micro-typography: 9–10px uppercase labels with wide letter-spacing

---

## 🛠️ Technologies Used

| Category | Technology | Version | Purpose |
|----------|-----------|---------|---------|
| **Framework** | Next.js | 16.2.9 | React framework with App Router |
| **UI Library** | React | 19.2.4 | Component-based UI |
| **Language** | TypeScript | 5.x | Type-safe development |
| **3D Engine** | Three.js | 0.185.0 | WebGL ocean scene rendering |
| **3D React** | React Three Fiber | 9.6.1 | React renderer for Three.js |
| **3D Helpers** | Drei | 10.7.7 | Three.js utilities (Points, PointMaterial) |
| **Animation** | GSAP | 3.15.0 | ScrollTrigger, tweens, marquee |
| **GSAP React** | @gsap/react | 2.1.2 | GSAP React integration |
| **Styling** | Tailwind CSS | v4 | Utility-first CSS framework |
| **PostCSS** | @tailwindcss/postcss | v4 | Tailwind CSS build plugin |

---

## 🔧 Tools and Frameworks

- **Next.js 16 (App Router)** — Server and client component architecture with automatic code splitting
- **GSAP ScrollTrigger** — Scroll-linked animations with scrub for frame-by-frame playback
- **React Three Fiber + Drei** — Declarative Three.js scenes with React component patterns
- **Tailwind CSS v4** — Utility classes combined with CSS custom properties via `@theme`
- **Canvas API** — Direct 2D canvas rendering for scroll-driven frame sequences
- **ESLint** — Code quality with `eslint-config-next` (core-web-vitals + TypeScript presets)
- **Google Fonts** — Inter and Playfair Display loaded via `<link>` tags

---

## 🏗️ Project Architecture

The project follows the **Next.js App Router** pattern with a single-page layout:

```
┌─────────────────────────────────────────────────────┐
│                    layout.tsx                        │
│  ┌───────────────────────────────────────────────┐  │
│  │  Google Fonts + Film Grain Overlay + Metadata │  │
│  └───────────────────────────────────────────────┘  │
│                    page.tsx                          │
│  ┌───────────────────────────────────────────────┐  │
│  │  Preloader                                    │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Fixed Nav Bar (glassmorphism)                │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Hero Scroll Canvas (300 frames + stories)    │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Bottom Ticker Marquee                        │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Feature Cards (interactive 3D expand)        │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Pool & Lifestyle Gallery (bento grid)        │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Fifth Scroll Canvas (300 frames)             │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Dining Marquee Gallery (CSS infinite scroll) │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Nightlife Bento Grid                         │  │
│  ├───────────────────────────────────────────────┤  │
│  │  About & Stats (3D tilt card)                 │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Third Scroll Canvas (300 frames + stories)   │  │
│  ├───────────────────────────────────────────────┤  │
│  │  Plan Your Visit (info grid + CTA)            │  │
│  └───────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────┘
```

**Component Strategy:**
- Scroll canvas components are **dynamically imported** with `ssr: false` to prevent server-side rendering of canvas/WebGL elements
- All interactive components are **client components** (`"use client"`)
- Static content and layout remain server-rendered for optimal initial load

---

## 📁 Folder Structure

```
cafe-3d-scroll-main/
├── public/
│   ├── designed for better experinece/   # Nightlife & experience photos (8 JPG + 7 JPEG)
│   ├── fifith scroll section/            # 300 animation frames (JPG sequence)
│   ├── food/                             # Fine dining photography (8 JPG)
│   ├── hero section scroll/              # 300 hero animation frames (JPG sequence)
│   ├── ship models/                      # Ship photography (4 JPG)
│   ├── the space/                        # Pool & lifestyle images (6 images)
│   └── UI layout/                        # Design reference screenshots (4 PNG)
│
├── src/
│   └── app/
│       ├── layout.tsx                    # Root layout (fonts, metadata, grain overlay)
│       ├── page.tsx                      # Main page (assembles all sections)
│       ├── globals.css                   # Global styles, animations, Tailwind theme
│       │
│       ├── ScrollCanvas.tsx              # Hero scroll frame animation (300 frames)
│       ├── CanvasWrapper.tsx             # Dynamic import wrapper (SSR disabled)
│       ├── ThirdScrollCanvas.tsx         # Third section frame animation
│       ├── ThirdCanvasWrapper.tsx        # Dynamic import wrapper
│       ├── FifthScrollCanvas.tsx         # Fifth section frame animation
│       ├── FifthCanvasWrapper.tsx        # Dynamic import wrapper
│       ├── CookingScrollCanvas.tsx       # Kitchen/cooking frame animation
│       ├── CookingCanvasWrapper.tsx      # Dynamic import wrapper
│       │
│       ├── OceanScene.tsx               # 3D WebGL ocean (Three.js)
│       ├── OceanSceneWrapper.tsx         # Dynamic import wrapper
│       │
│       ├── FeatureCards.tsx              # Interactive 3D expanding cards
│       ├── NightlifeBento.tsx            # Nightlife bento grid gallery
│       ├── PoolGallery.tsx              # Pool & lifestyle grid
│       ├── AboutStats.tsx               # About section with 3D tilt card
│       ├── Preloader.tsx                # Branded loading screen
│       │
│       ├── SpaceMarquee.tsx             # GSAP-powered image marquee
│       ├── ExpandingGallery.tsx          # Accordion-style image gallery
│       ├── BentoSection.tsx             # 3D perspective bento cards
│       └── SiteAnimations.tsx           # Global GSAP animation controller
│
├── next.config.ts                       # Next.js configuration
├── tsconfig.json                        # TypeScript configuration
├── postcss.config.mjs                   # PostCSS / Tailwind plugin
├── eslint.config.mjs                    # ESLint configuration
├── tailwind.config.ts                   # Tailwind CSS configuration
├── package.json                         # Dependencies and scripts
└── .gitignore                           # Git ignore rules
```

---

## 🚀 Installation and Setup

### Prerequisites

Ensure you have the following installed on your machine:

| Requirement | Minimum Version |
|-------------|----------------|
| **Node.js** | 18.x or higher |
| **npm** | 9.x or higher |
| **Git** | 2.x or higher |
| **Modern Browser** | Chrome, Firefox, Edge, or Safari with WebGL support |

### Step-by-Step Installation

**1. Clone the repository:**

```bash
git clone https://github.com/your-username/cafe-3d-scroll.git
cd cafe-3d-scroll
```

**2. Install dependencies:**

```bash
npm install
```

**3. Start the development server:**

```bash
npm run dev
```

**4. Open in your browser:**

Navigate to [http://localhost:3000](http://localhost:3000)

---

## ▶️ How to Run the Project

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with Turbopack (hot reload) |
| `npm run build` | Create optimized production build |
| `npm run start` | Serve the production build locally |
| `npm run lint` | Run ESLint for code quality checks |

### Production Build

```bash
npm run build
npm run start
```

The production server will be available at [http://localhost:3000](http://localhost:3000).

---

## ⚙️ Configuration and Environment Variables

This project is a **fully static front-end application** — no environment variables, API keys, or external service configuration is required.

**Key configuration files:**

| File | Purpose |
|------|---------|
| `next.config.ts` | Next.js settings (`ignoreBuildErrors: true` for TypeScript) |
| `tsconfig.json` | TypeScript compiler options, path alias `@/*` → `./src/*` |
| `postcss.config.mjs` | Tailwind CSS PostCSS plugin |
| `eslint.config.mjs` | ESLint rules (Next.js core-web-vitals + TypeScript) |

---

## 📖 Usage Instructions

1. **Open the website** — The preloader displays the NAVIS branding with an animated progress bar
2. **Scroll down** — The hero section begins a cinematic frame-by-frame animation as you scroll, with story panels appearing at key moments
3. **Explore feature cards** — Hover over the cards in the "Everything You Need At Sea" section to see them expand with 3D tilt effects
4. **Browse galleries** — The pool gallery and nightlife bento grids reveal content on hover with smooth transitions
5. **Continue scrolling** — Additional scroll-animated sections showcase craftsmanship and the NAVIS experience
6. **View dining** — The dining marquee continuously scrolls through fine dining photography
7. **Reach the footer** — The "Plan Your Visit" section provides departure information and a call-to-action

> **💡 Tip:** For the best experience, use a mouse or trackpad with smooth scrolling. The scroll-driven animations are designed for gradual, continuous scroll input.

---

## 🔮 Future Enhancements

- **Mobile Responsiveness** — Add full responsive breakpoints for all grid layouts and a hamburger navigation menu
- **Smooth Scroll Integration** — Activate the installed Lenis library for buttery-smooth scroll behavior
- **Page Transitions** — Leverage the installed Framer Motion library for route transition animations
- **Performance Optimization** — Implement lazy loading for frame sequences and progressive image loading
- **Additional Pages** — Expand into multi-page routing (Voyages, Experience, About, Contact)
- **Booking System** — Add an interactive voyage booking flow with date selection and cabin options
- **Accessibility** — Implement ARIA labels, keyboard navigation, and reduced-motion preferences
- **SEO Enhancement** — Add structured data, Open Graph meta tags, and dynamic sitemap generation
- **Testing** — Write end-to-end tests using the installed Playwright framework

---

## 🤝 Contributing Guidelines

Contributions are welcome! Follow these steps to contribute:

1. **Fork** the repository
2. **Create** a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit** your changes with descriptive messages:
   ```bash
   git commit -m "Add: description of your changes"
   ```
4. **Push** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** with a clear description of the changes

### Code Standards

- Follow the existing code style and component patterns
- Use TypeScript for all new files
- Ensure ESLint passes (`npm run lint`)
- Test on multiple browsers and screen sizes
- Do not commit `node_modules/`, `.next/`, or environment files

---

<div align="center">

**Built with ❤️ using Next.js, Three.js, and GSAP**

⭐ Star this repository if you found it interesting!

</div>

