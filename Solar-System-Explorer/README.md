# ASTRA — Solar System & ISRO 3D Mission Explorer

## ISRO Earth-orbit showcase
This build displays **20 individually modelled ISRO spacecraft around a 3D Earth at the same time**. The models are generated as 3D WebGL geometry; they are not 20 copies of one satellite mesh and are not flat satellite photographs pasted into the scene.

Each model has a mission-family silhouette and distinctive payload geometry: communications reflectors, optical telescopes, radar apertures/booms, navigation antennas, ocean-observation instruments, scientific telescopes, solar wings and different spacecraft bus shapes. Select a mission in the catalogue to focus its 3D model and open its mission dossier with the available mission image and source attribution.

### The 20 Earth-orbit missions
Aryabhata; Bhaskara-1; INSAT-1B; IRS-1A; Cartosat-1; Cartosat-2; Oceansat-2; GSAT-6; GSAT-7; GSAT-19; IRNSS-1B; NVS-01; Cartosat-3; Resourcesat-2A; RISAT-1; INSAT-3DS; Megha-Tropiques; AstroSat; XPoSat; NISAR.

### Important scientific note
The Earth scene is an **educational orbit showcase**, not a literal real-time ephemeris display. The 20 models are intentionally arranged around Earth so that every spacecraft can be seen together. Their orbit radii, plane orientations, spacing and speeds are illustrative and are not to scale or date-accurate. Some historical spacecraft have completed their missions or re-entered; the scene does not imply that all 20 are currently operating or still in orbit. The dossier gives the documented historical orbit and status where available.

### 3D model accuracy
The 3D spacecraft are mission-inspired visual reconstructions based on documented mission roles and payload families. They are **not engineering-grade CAD replicas** unless explicitly identified as such. A real mission photograph/rendering is shown in the dossier where an attributable image is available; it is not reused as the 3D model.

## Run locally
1. Extract the ZIP.
2. Open the `Solar-System-Explorer` folder in VS Code.
3. Open `index.html` with Live Server.
4. The interactive `INDIA IN SPACE · ISRO` scene opens by default, with 20 distinct ISRO spacecraft orbiting Earth and an India marker on the globe.
5. Select a mission from the left catalogue to open its dossier and focus its spacecraft.

No external 3D library or CDN is required. The 3D renderer is WebGL. Some dossier images are loaded from official ISRO or credited public image sources and therefore need an internet connection.

## Controls
- Drag to rotate the camera.
- Scroll or use zoom buttons to zoom.
- Select a mission in the sidebar to focus its 3D model.
- Use pause, reset and orbit toggles.

## Main source files
- `js/main.js`: WebGL rendering, 20 unique model assemblies, camera and interaction.
- `js/data/isro-catalog.js`: selected mission facts, payloads, roles, working principles, applications and sources.
- `js/data/mission-images.js`: image-selection helper.
- `index.html`, `style.css`: interface and responsive styling.

## Sources
Mission facts are linked to official ISRO mission pages in each dossier. The 3D geometry is an educational visual interpretation and should not be used as an engineering reference.
