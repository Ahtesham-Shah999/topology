# 🌌 Lumina WebGL: Interactive 3D Topology Experience

<div align="center">

![WebGL](https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-Custom_Fonts-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**A highly customized, interactive 3D WebGL experience featuring topographical data rendering and precision typography.**

[✨ Features](#-key-features) • [🏗️ Architecture](#-technical-architecture) • [🚀 Quick Start](#-quick-start) • [🗂️ Structure](#-project-structure)

</div>

---

## 📌 Overview

**Lumina WebGL** (internally referenced as *topology_font_updated99*) is a bespoke front-end rendering engine built for a high-profile client. 

The application utilizes **Three.js** and **WebGL** to render interactive 3D topologies directly in the browser, overlaid with pixel-perfect custom typography (`Magnetik`, `Space Mono`, and `Lazare Grotesk`) designed strictly to the client's design specifications.

### 🌟 Key Features
- **3D Topology Rendering:** Utilizes WebGL shaders to map and render complex 3D topographical surfaces.
- **Precision Typography:** Implements strict CSS overrides for font-faces (`Magnetik` for headings, `Space Mono` for body text) ensuring brand consistency over the 3D canvas.
- **High-Performance Canvas:** Optimized asset loading and preloading of `.woff2` font files to prevent layout shifts (CLS) and ensure rapid Time-to-Interactive (TTI).
- **Analytics Integrated:** Pre-configured Google Tag Manager (GTAG) with GDPR-compliant cookie consent handling.

---

## 🏗️ Technical Architecture

This project is delivered as a pre-compiled, highly optimized static bundle.

- **Graphics Engine:** Three.js / WebGL context mounted to a root DOM element.
- **Asset Pipeline:** The project utilizes a modern bundler (Vite/Webpack) to output heavily minified CSS and JS chunks (e.g., `index-CYsj0Cs1.js`).
- **Typography Injection:** Custom `@font-face` rules are injected directly into the HTML `<style>` head with strict `!important` flags to guarantee the client's typography renders correctly across all viewports and browsers, completely independent of the WebGL context.

---

## 🚀 Quick Start

Because the assets are pre-compiled for production, you can run the experience instantly using a lightweight local web server.

### 1. Clone the repository
```bash
git clone https://github.com/Ahtesham-Shah999/topology_font_updated99.git
cd topology_font_updated99
```

### 2. Start the Local Server
The project includes a package.json script that utilizes Python's built-in HTTP server to serve the `public` directory.

```bash
npm run dev
# OR manually:
python -m http.server 8000 --directory public
```

### 3. View the Experience
Open your browser and navigate to:
**http://localhost:8000**

---

## 🗂️ Project Structure

```text
Lumina-WebGL/
├── public/
│   ├── index.html        # Entry point containing GTAGs, CSS font overrides, and the WebGL root
│   ├── build/            # Minified JS/CSS bundles and .woff2 custom font files
│   ├── images/           # Favicons and manifest files for PWA compatibility
│   └── webgl/            # Core 3D geometry, shaders, and topology assets
├── package.json          # Server runtime scripts
└── README.md             # Project documentation
```

---

## 🧠 Technical Highlights for Recruiters

- **WebGL / Three.js Mastery:** Demonstrates the ability to integrate heavy 3D rendering contexts cleanly into the browser DOM without compromising UI performance.
- **Client-Driven Typography:** Shows strict adherence to design requirements, utilizing advanced CSS font preloading to eliminate FOUT (Flash of Unstyled Text) over a 3D canvas.
- **Production-Ready Bundles:** Code is securely bundled, minified, and optimized for immediate static deployment on platforms like Vercel, Netlify, or AWS S3.

---

## 👨‍💻 Developer

**Ahtesham Shah**
- 🌐 [GitHub](https://github.com/Ahtesham-Shah999)
- 💼 3D Web/WebGL & Frontend Engineer

---

<div align="center">
  <i>⭐ Bringing complex data and beautiful design to the 3D web.</i>
</div>