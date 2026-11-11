# Cube Maker 3D for After Effects (v1.3)

[![Live Browser Simulator](https://img.shields.io/badge/Live%20Demo-AE%20ScriptUI%20Simulator-2c8cff?style=for-the-badge&logo=javascript)](https://work2survive.github.io/AE_JS_builder/?jsx=cube_maker.jsx)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)
[![Adobe After Effects](https://img.shields.io/badge/Adobe%20After%20Effects-CS6%20--%20CC%202026%2B-9999FF?style=for-the-badge&logo=adobeaftereffects)](https://www.adobe.com/products/aftereffects.html)

A versatile, parametric Adobe After Effects ScriptUI panel that generates, builds, and dynamically rigs 3D Cubes and rectangular solids with independent face colors, opacity, and stroke controls.

> **Live Browser Simulator**: Test and preview this tool interactively in the [AE JS & ScriptUI Simulator](https://work2survive.github.io/AE_JS_builder/?jsx=cube_maker.jsx) directly in your web browser without launching After Effects!

---

## ✨ Features

### 1. Geometry & Dimensions
- **Dimensions (X, Y, Z)**: Scrubbable sliders and numerical inputs for width, height, and depth (10 to 500 px).
- **Link All Sizes to Z**: Checkbox adding an AE Checkbox Control effect. When checked, links X and Y dimensions to Z depth. Supports timeline keyframing and expressions.
- **Topology & Precomp**: Builds 6 rectangular shape faces parented to a master controller, precomposed into a clean subcomp with continuous rasterization (`collapseTransformation = true`).

### 2. Appearance & Styling
- **Face & Edge Colors**: Live color swatches paired with direct hex inputs for sides fill and border stroke.
- **Opacity Controls**: Independent sliders for Face Opacity (0–100%) and Stroke Opacity (0–100%).
- **Stroke Width**: Real-time slider (0 to 20 px) with automatic stroke suppression when width is 0.
- **Corner Roundness & Face Gap**: Scrubbable sliders for rounded bevels and inset edge spacing.

### 3. Master Rigging
- Adds Master Effect Controls to the precomposition layer in the host comp, giving animators single-point control over all 6 3D faces without diving inside nested comps.

---

## 🚀 Installation & Usage

1. Download [`cube_maker.jsx`](cube_maker.jsx).
2. Place it in your After Effects Scripts folder:
   - **Windows**: `C:\Program Files\Adobe\Adobe After Effects <Version>\Support Files\Scripts\ScriptUI Panels\`
   - **macOS**: `/Applications/Adobe After Effects <Version>/Scripts/ScriptUI Panels/`
3. Restart After Effects or launch via **File > Scripts > Run Script File...**
4. In After Effects, open **Window > cube_maker.jsx**.

---

## 📄 License

MIT License. Copyright (c) 2026 [work2survive](https://github.com/work2survive).
