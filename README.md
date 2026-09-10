# AURA MOTORS — Interactive 3D Luxury Car Showcase

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![Deployment](https://img.shields.io/badge/Deployment-GitHub%20Pages-success?style=for-the-badge&logo=github)](https://pages.github.com/)

**AURA MOTORS** is an interactive luxury car dealership experience built around immersive 3D vehicle exploration.
Browse vehicles, inspect performance specifications, rotate cars in 360°, and explore a premium dark-mode showroom interface designed for modern browsers.

**[Live Demo](#) | [Report Bug](../../issues/new) | [Request Feature](../../issues/new)**

---

## ✨ Preview

<p align="center">
  <img src="assets/aura-motors-featured-machine.webp" alt="AURA MOTORS Featured Machine" width="900">
</p>

<p align="center">
  <img src="assets/aura-motors-homepage.webp" alt="AURA MOTORS Homepage and Interactive 3D Experience" width="900">
</p>

---

## 🚘 Key Features

- **360° 3D Interactivity** — Rotate and inspect vehicles directly in the browser using interactive `.glb` models.
- **Luxury Visual Design** — Deep burgundy accents, dark backgrounds, subtle glow effects, metallic styling, and premium typography.
- **Responsive Layout** — Designed to provide a polished experience across desktop, tablet, and mobile screens.
- **Full-Screen 3D Viewer** — Open vehicles in an expanded modal for a more immersive showroom experience.
- **Performance Specifications** — Display key vehicle information such as horsepower, acceleration, top speed, and drivetrain.
- **Showroom Grid** — Browse featured vehicles through a structured luxury dealership layout.
- **Test-Drive Booking** — Built-in contact and test-drive form for potential customers.
- **Graceful 3D Fallbacks** — Handles failed model loading without allowing the interface to break.

---

## 🛠️ Tech Stack

| Technology | Version / Source | Implementation Purpose |
|---|---|---|
| **HTML5** | HTML5 | Application structure and semantic markup |
| **Tailwind CSS** | CDN | Utility-first styling and responsive layout |
| **Google Model Viewer** | `3.4.0` | Interactive 3D `.glb` model rendering |
| **Google Fonts — Cinzel** | Google Fonts | Luxury display typography |
| **Google Fonts — Plus Jakarta Sans** | Google Fonts | Modern UI and body typography |
| **GLB / glTF** | Binary glTF | Self-contained 3D vehicle assets |

---

## 🚀 Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/AnuraagMoharana/Luxury-Car-Dealership.git
cd Luxury-Car-Dealership
```

### 2. Open the project

The application is primarily contained in:

```text
index.html
```

For the best local development experience, use **VS Code + Live Server**.

### 3. Run with Live Server

Install the **Live Server** extension in VS Code, then:

1. Open the project folder.
2. Right-click `index.html`.
3. Select **Open with Live Server**.
4. Your browser will open the AURA MOTORS showroom.

### Alternative

You can also open `index.html` directly in a modern browser, although using a local development server is recommended for consistent asset loading.

---

## 🏎️ Replacing 3D Car Models

AURA MOTORS uses Google's `<model-viewer>` component to display `.glb` files.

Locate the existing model URL:

```html
<model-viewer
  src="https://example.com/car-model.glb"
  camera-controls
  auto-rotate
  shadow-intensity="1"
  exposure="1"
  alt="Luxury sports car">
</model-viewer>
```

Replace the `src` value with your own `.glb` file:

```html
<model-viewer
  src="./assets/my-luxury-car.glb"
  camera-controls
  auto-rotate
  shadow-intensity="1"
  exposure="1"
  alt="My luxury car">
</model-viewer>
```

### Recommended `.glb` setup

```text
assets/
├── car-one.glb
├── car-two.glb
└── car-three.glb
```

Then reference them from HTML:

```html
<model-viewer src="./assets/car-one.glb"></model-viewer>
<model-viewer src="./assets/car-two.glb"></model-viewer>
<model-viewer src="./assets/car-three.glb"></model-viewer>
```

Using a single `.glb` file is convenient because the binary glTF format can package the model and its associated resources together.

---

## 📁 Folder Structure

```text
Luxury-Car-Dealership/
│
├── index.html
├── README.md
│
└── assets/
    ├── aura-motors-featured-machine.webp
    └── aura-motors-homepage.webp
```

> The current implementation can also load publicly hosted `.glb` assets directly, so the `assets/` directory is optional unless you want to self-host your models.

---

## 🎨 Design System

### Primary Aesthetic

```text
Theme       → Luxury Dark Mode
Accent      → Burgundy #800020
Typography  → Cinzel + Plus Jakarta Sans
Style       → Premium / Minimal / Automotive
Effects     → Glow, shadows, metallic highlights
```

The interface is designed to feel closer to a premium automotive configurator than a conventional dealership website.

---

## 🌐 Deployment

The project is compatible with static hosting platforms such as:

- **GitHub Pages**
- **Netlify**
- **Vercel**
- **Cloudflare Pages**

For GitHub Pages, push the repository to GitHub and configure Pages to deploy from the repository's main branch.

---

## 📜 License

This project is released under the **MIT License**.

You are free to use, modify, distribute, and build upon the source code, subject to the terms of the license.

See [`LICENSE`](LICENSE) for the complete license text.

---

## 🙏 Acknowledgments

- **Google Model Viewer** — Used for browser-based interactive 3D rendering.
- **Tailwind CSS** — Used for responsive utility-based styling.
- **Google Fonts** — Cinzel and Plus Jakarta Sans provide the project's typography.
- **Khronos glTF Sample Assets** — Public 3D assets may be used as demonstration models where applicable and according to their respective licenses.

---

## ⭐ Project

**AURA MOTORS — Engineering Perfection**

Built as a modern concept for an immersive, luxury automotive dealership experience. 🚘✨
