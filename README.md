
# ASTRA — Solar System & ISRO Satellite Explorer

### Explore the Universe. Discover India's Space Technology.

ASTRA is an interactive 3D space exploration web application built using HTML5, CSS3, JavaScript, and Pure WebGL. It allows users to explore the Solar System, interact with 3D planets, discover scientific information, and visualize 20 distinct ISRO spacecraft models orbiting a 3D Earth.

The project combines real-time 3D rendering, interactive camera controls, astronomical information, satellite-inspired 3D models, and an immersive space-themed interface into one platform.

---

## 🚀 Live Demo

**Live Website:** https://fluffy-tarsier-98ce2b.netlify.app

**GitHub Repository:** https://github.com/bodigeashritha22/solar-system-explorer-isro

---

## 🌌 Project Overview

ASTRA provides two major exploration experiences:

### 1. Solar System Explorer

Explore the eight planets of our Solar System through an interactive 3D environment.

Features include:
- Interactive 3D Solar System visualization.
- Eight planets with individual 3D appearances.
- Planet selection and exploration.
- Planet information panels.
- Planetary rotation and orbital animation.
- Interactive camera movement and zoom.
- Space-themed background and star visualization.
- Detailed astronomical information.

### 2. ISRO Satellite Explorer

Discover Indian Space Research Organisation (ISRO) spacecraft through an interactive 3D Earth visualization.

The satellite explorer features 20 distinct mission-inspired 3D spacecraft models positioned around Earth.

Features include:
- Interactive 3D Earth.
- Twenty different satellite-inspired 3D models.
- Multiple orbital paths and orbital orientations.
- Animated satellite movement.
- Individual satellite selection.
- Satellite mission information.
- Mission reference photographs.
- Launch details and spacecraft specifications.
- Mission objectives and applications.
- Camera focus and reset controls.

**Important:** The satellite models are custom, mission-inspired visual reconstructions rather than engineering-grade CAD models. Their orbital positions and motion are illustrative, not live orbital tracking. Historical spacecraft are included for educational purposes and are not necessarily operational today.

---

## 🛰️ Featured ISRO Spacecraft

The project includes the following 20 spacecraft:

| No. | Spacecraft | Primary Mission |
|---|---|---|
| 1 | Aryabhata | India's first satellite |
| 2 | Bhaskara-1 | Earth observation |
| 3 | INSAT-1B | Communication and meteorology |
| 4 | GSAT-6 | Communication |
| 5 | GSAT-19 | Communication technology |
| 6 | IRNSS-1B | Navigation |
| 7 | NVS-01 | Navigation |
| 8 | Cartosat-3 | High-resolution Earth observation |
| 9 | Resourcesat-2A | Natural resource monitoring |
| 10 | RISAT-1 | Radar imaging |
| 11 | INSAT-3DS | Meteorological observation |
| 12 | Megha-Tropiques | Tropical weather and climate research |
| 13 | AstroSat | Space astronomy |
| 14 | XPoSat | X-ray polarimetry |
| 15 | NISAR | Earth observation using radar |
| 16 | IRS-1A | Remote sensing |
| 17 | Cartosat-1 | Stereo Earth imaging |
| 18 | Cartosat-2 | High-resolution imaging |
| 19 | Oceansat-2 | Ocean observation |
| 20 | GSAT-7 | Maritime communication |

The collection includes historical and more recent missions. It does not imply that all spacecraft are currently operational or orbiting Earth today.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling, layouts, animations and responsive design |
| JavaScript (ES6+) | Application logic and interactions |
| WebGL 1.0 | Hardware-accelerated 3D rendering |
| GLSL | Vertex and fragment shaders |
| HTML Canvas | Rendering surface |
| Git | Version control |
| GitHub | Source code hosting |
| Vercel | Website deployment |

**Rendering approach:** Pure WebGL. The application uses custom WebGL rendering logic and GLSL shaders rather than depending on Three.js.

---

## ⚙️ Core Implementation

### 1. WebGL Rendering

WebGL renders 3D objects directly inside the HTML canvas using the browser's graphics capabilities.

The application uses:
- WebGL context initialization.
- Vertex buffers and index buffers.
- Vertex and fragment shaders.
- Projection and model-view transformations.
- Texture mapping.
- Depth testing.
- Lighting calculations.
- Animation loops.

### 2. GLSL Shaders

GLSL is used to control how 3D objects are rendered.

**Vertex Shader:**
- Processes 3D vertex positions.
- Applies model, view and projection transformations.
- Passes information to the fragment shader.

**Fragment Shader:**
- Calculates pixel colours.
- Applies texture and lighting effects.
- Produces the final rendered appearance.

### 3. 3D Geometry

The application uses reusable geometry to construct 3D objects.

Examples include:
- Spheres for planets and Earth.
- Cubes for satellite bodies.
- Cylinders for spacecraft components.
- Panels for solar arrays.
- Antenna and dish structures.
- Orbital paths.

Different combinations of these geometries create distinct satellite-inspired models.

### 4. Animation

JavaScript animation updates object positions and rotations over time.

The animation system supports:
- Planet rotation.
- Planetary orbital movement.
- Earth rotation.
- Satellite orbital movement.
- Satellite model rotation.
- Continuous rendering.

### 5. Camera Controls

The camera system enables users to explore the 3D environment.

It supports:
- Zooming.
- Camera movement.
- Object focus.
- Satellite selection.
- Camera reset.

---

## 📂 Project Structure

```text
Solar-System-Explorer/
│
├── index.html
│
├── style.css
│
├── README.md
│
├── js/
│   ├── main.js
│   │
│   └── data/
│       ├── isro-catalog.js
│       └── mission-images.js
│
└── assets/
    └── images/
        └── satellite-fallback.svg
```

### File Descriptions

**index.html**
- Main application structure.
- Canvas element for WebGL rendering.
- Navigation and interface elements.
- Information panels.

**style.css**
- Application layout and visual styling.
- Space-themed interface.
- Responsive design.
- Interactive visual effects.

**js/main.js**
- WebGL initialization.
- Shader programs.
- 3D geometry generation.
- Planet and satellite rendering.
- Camera controls.
- Animation loop.
- User interaction handling.

**js/data/isro-catalog.js**
- ISRO spacecraft catalogue.
- Mission descriptions.
- Launch information.
- Orbit and payload details.
- Mission objectives.

**js/data/mission-images.js**
- Satellite mission image handling.

**assets/images/**
- Local image assets and fallback graphics.

---

## ▶️ How to Run Locally

### Requirements

- A modern web browser.
- Visual Studio Code.
- VS Code Live Server extension.
- Git (optional).

### Steps

1. Download or clone the repository.

```bash
git clone https://github.com/bodigeashritha22/solar-system-explorer-isro.git
```

2. Open the project folder in Visual Studio Code.

3. Open the `Solar-System-Explorer` folder if the repository contains the project inside it.

4. Open `index.html`.

5. Right-click and select **Open with Live Server**.

6. Explore the Solar System and ISRO Satellite Explorer.

Use a browser with WebGL support and hardware acceleration enabled for the best experience.

---

## 🌐 Deployment

The project can be deployed using Vercel.

### Deployment Steps

1. Push the project to GitHub.
2. Open https://vercel.com/
3. Sign in using GitHub.
4. Select **Add New Project**.
5. Import the `solar-system-explorer-isro` repository.
6. Configure the project:

| Configuration | Value |
|---|---|
| Framework Preset | Other |
| Root Directory | `Solar-System-Explorer` |
| Build Command | Leave empty |
| Output Directory | `.` |
| Install Command | Leave empty |

7. Click **Deploy**.

Vercel will generate a public deployment URL.

---

## 📚 Information Sources

Mission information should be cross-checked with official ISRO resources.

- ISRO: https://www.isro.gov.in/
- ISRO Missions: https://www.isro.gov.in/Spacecraft.html
- ISRO Earth Observation: https://www.isro.gov.in/
- MOSDAC: https://mosdac.gov.in/
- NASA Solar System Exploration: https://science.nasa.gov/solar-system/

Satellite photographs are provided as mission reference images. Their original publishers and image credits should be respected.

---

## 🎯 Project Objectives

- Demonstrate interactive 3D graphics using Pure WebGL.
- Understand the fundamentals of computer graphics.
- Explore planetary motion and astronomical objects.
- Present India's satellite missions in an interactive environment.
- Demonstrate JavaScript animation and event handling.
- Combine scientific information with interactive visualization.
- Build a responsive and immersive educational web application.

---

## 🔮 Future Enhancements

Potential improvements include:

- Real-time satellite tracking using orbital TLE data.
- Integration with satellite tracking APIs.
- More detailed planetary surface textures.
- Realistic Earth clouds and atmospheric effects.
- More accurate spacecraft 3D models.
- Moon and planetary satellite systems.
- Detailed mission timelines.
- Search and filter for spacecraft.
- Additional ISRO launch vehicle visualizations.
- Mobile and touch-friendly camera controls.

---

## ⚠️ Important Notes

- Satellite models are educational, mission-inspired 3D reconstructions, not exact spacecraft engineering models.
- The displayed orbital arrangement is illustrative and not to scale.
- Satellite positions are not connected to live orbital tracking data.
- Mission status should be checked against official ISRO sources.
- Historical missions are included for educational exploration.
- Visual appearance depends on the browser, graphics hardware and WebGL support.

---

## 👩‍💻 Developer

**Developed by:** Ashritha Bodige

**Project:** ASTRA – Solar System & ISRO Satellite Explorer

**Domain:** Web Development | Computer Graphics | Space Technology

**GitHub:** https://github.com/bodigeashritha22

---

## ⭐ Support

If you find this project interesting, consider giving the repository a star on GitHub.

**Explore the planets. Discover the missions. Experience space through ASTRA.**
