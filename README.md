# AE Cube Maker 3D (v1.3)

[![Live Browser Simulator](https://img.shields.io/badge/Live%20Demo-AE%20ScriptUI%20Simulator-2c8cff?style=for-the-badge&logo=javascript)](https://work2survive.github.io/AE_JS_builder/?jsx=cube_maker.jsx)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)
[![Adobe After Effects](https://img.shields.io/badge/Adobe%20After%20Effects-CS6%20--%20CC%202026%2B-9999FF?style=for-the-badge&logo=adobeaftereffects)](https://www.adobe.com/products/aftereffects.html)

An interactive, parametric Adobe After Effects ScriptUI panel that creates, configures, and dynamically rigs 3D Cubes and rectangular solids built entirely out of native After Effects Shape Layers.

> **Live Browser Simulator**: Test and preview this tool interactively in the [AE JS & ScriptUI Simulator](https://work2survive.github.io/AE_JS_builder/?jsx=cube_maker.jsx) directly in your web browser without launching After Effects!

---

## ✨ Features

### 1. Geometry & Dimensions
- **Dimensions (X, Y, Z)**: Scrubbable sliders and numerical edit text inputs ($10\text{ to }500\text{ px}$) for independent width, height, and depth control.
- **Link All Sizes to Z**: One-click checkbox adding an AE Checkbox Control effect. When checked, links X and Y dimensions directly to Z depth for uniform cubic scaling. Supports timeline keyframing and expressions.
- **3D Topology & Precomposition**: Builds 6 rectangular shape faces (Front, Back, Left, Right, Top, Bottom) parented to a master controller layer, precomposed into an auto-rigged subcomp with continuous rasterization (`collapseTransformation = true`).

### 2. Appearance & Styling
- **Face & Edge Colors**: Live rectangular color swatches paired with direct hex inputs (`#RRGGBB`) with integrated Windows Color Picker and After Effects native color dialog support.
- **Independent Opacity Controls**: Scrubbable sliders for Face Opacity ($0\text{--}100\%$) and Stroke Opacity ($0\text{--}100\%$).
- **Stroke Width**: Real-time slider ($0\text{ to }20\text{ px}$) with automatic stroke suppression when width is 0.
- **Corner Roundness & Face Gap**: Scrubbable sliders for rounded beveled corners ($0\text{ to }80\text{ px}$) and inset face edge spacing ($0\text{ to }40\text{ px}$) to create tech grids, sci-fi panels, and floating tile blocks.

### 3. Master Rigging & Timeline Animation
- **Single-Point Timeline Control**: Exposes Master Effect Controls on the parent precomp layer in the host composition, giving animators full control over all 6 3D faces without diving inside nested subcomps.
- **Dual Classification Color Coding**:
  - 🔵 **Animatable Properties**: Properties that can be animated in the timeline (Dimensions, Colors, Stroke Width, Opacities).
  - 🔴 **Structural Properties**: Properties defined once upon script setup (Cube Structure, 3D Topology, Build/Reset button).
- **MOGRT / Essential Graphics Ready**: All controls can be directly added to the Essential Graphics panel for Adobe Premiere Pro motion graphic templates.

---

## 🎛️ Exposed Controls Reference

Once created, the master layer contains the following controls:

| Control Name | Type | Description |
|---|---|---|
| **Size X** | Slider Control | Cube width in pixels ($10\text{--}500\text{ px}$). |
| **Size Y** | Slider Control | Cube height in pixels ($10\text{--}500\text{ px}$). |
| **Size Z** | Slider Control | Cube depth in pixels ($10\text{--}500\text{ px}$). |
| **Link all sizes to Z** | Checkbox Control | When checked ($1$), forces Size X and Y to follow Size Z. |
| **Sides Color** | Color Control | RGB fill color for all 6 cube faces. |
| **Sides Opacity** | Slider Control | Fill opacity percentage ($0\text{--}100\%$). |
| **Stroke Color** | Color Control | Border stroke color for all 6 faces. |
| **Stroke Width** | Slider Control | Border stroke width in pixels ($0\text{--}20\text{ px}$). |
| **Stroke Opacity** | Slider Control | Border stroke opacity percentage ($0\text{--}100\%$). |
| **Corner Roundness** | Slider Control | Corner bevel radius on each face ($0\text{--}80\text{ px}$). |
| **Face Gap** | Slider Control | Inset margin distance between adjacent faces ($0\text{--}40\text{ px}$). |

---

## 🚀 Installation & Usage

### Option 1: Dockable Panel (Recommended)
1. Download [`cube_maker.jsx`](cube_maker.jsx).
2. Place it into your After Effects `ScriptUI Panels` directory:
   - **Windows**:
     ```text
     C:\Program Files\Adobe\Adobe After Effects <Version>\Support Files\Scripts\ScriptUI Panels\
     ```
   - **macOS**:
     ```text
     /Applications/Adobe After Effects <Version>/Scripts/ScriptUI Panels/
     ```
3. Restart After Effects.
4. Launch from the menu: **Window > cube_maker.jsx**.

### Option 2: Run Directly Without Installing
1. In After Effects, navigate to **File > Scripts > Run Script File...**
2. Browse to and select `cube_maker.jsx`.

---

## 💡 Use Cases

- **3D Motion Graphics & Product Showcases**: Generate isometric or perspective cubes, product packaging boxes, and tech cubes.
- **HUDs & UI Panels**: Use rounded faces with gap spacing to create holographic sci-fi cubes and HUD data cubes.
- **Dynamic Infographics**: Keyframe Size X, Y, and Z to animate 3D bar charts and spatial data blocks.

---

## 📄 License

MIT License. Copyright (c) 2026 [work2survive](https://github.com/work2survive).
