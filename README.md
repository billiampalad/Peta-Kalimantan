<div align="center">

# 🗺️ WebGIS Kalimantan: Spatial Cartography & Interactive Web Mapping

<p align="center">
  <strong>An interactive geospatial web application showcasing provincial administrative boundaries, urban population dispersion, and shaded relief across Kalimantan (Borneo), Indonesia.</strong>
</p>

[![Live Demo](https://img.shields.io/badge/Demo-Live%20Website-00C853?style=for-the-badge&logo=googlechrome&logoColor=white)](https://billiampalad.github.io/Peta-Kalimantan/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/billiampalad/Peta-Kalimantan)
[![QGIS](https://img.shields.io/badge/QGIS-3.x-589632?style=for-the-badge&logo=qgis&logoColor=white)](https://qgis.org/)
[![Leaflet](https://img.shields.io/badge/Leaflet-1.9.4-199900?style=for-the-badge&logo=leaflet&logoColor=white)](https://leafletjs.com/)
[![GeoJSON](https://img.shields.io/badge/Data-GeoJSON%20Vector-E65100?style=for-the-badge)](https://geojson.org/)

---

### 🌐 [Explore The Live Interactive Map ↗](https://billiampalad.github.io/Peta-Kalimantan/)

</div>

<br />

## 📖 Table of Contents
- [Overview](#-overview)
- [Project Metadata](#-project-metadata)
- [Key Features](#-key-features)
- [Geospatial Data & Layers](#-geospatial-data--layers)
- [Interactive Toolset](#-interactive-toolset)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)
- [Running Locally](#-running-locally-offline)
- [Author & Acknowledgments](#-author--acknowledgments)

---

## 🌟 Overview

**WebGIS Kalimantan Map** is an open-access web cartography project designed to visualize multi-layer geospatial data across Kalimantan (Borneo Island). 

Built through **QGIS** and exported using the **qgis2web** engine into a fully self-contained **Leaflet.js** web application, this platform allows users to explore administrative divisions, analyze demographic distribution across major cities, search places in real-time, and perform on-map spatial measurements.

> 💡 **Key Highlight:** Completely client-side and lightweight, requiring zero external backend services to explore the rich geographical datasets.

---

## 📌 Project Metadata

| Attribute | Details |
| :--- | :--- |
| **Course** | Geographic Information Systems (GIS) |
| **Topic** | Spatial Layouting, Thematic Cartography & WebGIS Publishing |
| **Study Region** | Kalimantan Island (Borneo), Indonesia |
| **Coordinate Reference System (CRS)** | `WGS 84 / CRS84` (EPSG: 4326) |
| **Lead Developer** | Clynten Billiam Palad |
| **Live Deployment** | [billiampalad.github.io/Peta-Kalimantan](https://billiampalad.github.io/Peta-Kalimantan/) |

---

## 🚀 Key Features

- 🏛️ **Provincial Administrative Hierarchy**: Detailed vector boundaries covering West, Central, South, East, and North Kalimantan.
- 🏙️ **Dynamic Demographic Classification**: Graduated circle symbols highlighting populated urban places scaled by population rank (`POP_MAX` / `POP_MIN`).
- 🌄 **Natural Topographic Basemap**: High-resolution Natural Earth shaded relief raster overlay with water bodies.
- 📐 **Geospatial Measurement Engine**: Accurate point-to-point distance calculations and polygon area measurements directly on the canvas.
- 🔍 **Integrated Geocoding**: Real-time location search powered by the Photon geocoder API.
- 🎛️ **Interactive Layer Management**: Full layer switcher allowing users to toggle boundaries, labels, and datasets dynamically.

---

## 🗂️ Geospatial Data & Layers

| Layer Identifier | Geometry Type | Data Provider | Description |
| :--- | :---: | :--- | :--- |
| `ne_10m_populated_places` | Point | Natural Earth (1:10m) | Major urban settlements classified by demographic size (*Pontianak, Samarinda, Balikpapan, Banjarmasin, Palangkaraya, Tarakan, etc.*) |
| `ne_10m_admin_1_states_provinces` | Polygon | Natural Earth (1:10m) | Provincial administrative borders across the Kalimantan region |
| `NE1_50M_SR_W` | Raster | Natural Earth (1:50m) | Surface terrain relief with integrated bathymetry & water bodies |

---

## 🛠️ Interactive Toolset

```
┌─────────────────────────────────────────────────────────────┐
│                      LEAFLET WEB CANVAS                     │
├───────────────────────────────┬─────────────────────────────┤
│ 🔍 Photon Geocoder            │ Search and fly to any place │
│ 📏 Leaflet Measure            │ Measure distances & areas   │
│ 🏷️ Labelgun & RBush Engine    │ Collision-free city labels  │
│ 💬 Dynamic Tooltips & Popups  │ Detailed attribute lookup   │
│ 🗂️ Layer Tree Controller      │ Toggle visual vector layers │
└───────────────────────────────┴─────────────────────────────┘
```

---

## 💻 Tech Stack

- **GIS Software**: [QGIS 3.x Desktop](https://qgis.org/)
- **Web Export Engine**: [qgis2web plugin](https://github.com/tomchadwin/qgis2web)
- **Web Mapping Library**: [Leaflet.js](https://leafletjs.com/)
- **Data Formats**: GeoJSON, Raster GeoTIFF / PNG, SVG Markers
- **Front-End**: HTML5, CSS3, Vanilla JavaScript
- **Hosting**: GitHub Pages

---

## 📂 Repository Structure

```plaintext
Peta-Kalimantan/
├── css/                   # Leaflet, Measure, and custom cartography styles
├── data/                  # Exported GeoJSON datasets & raster basemap
│   ├── NE1_50M_SR_W_0.png
│   ├── ne_10m_admin_1_states_provincescopy_1.js
│   └── ne_10m_populated_placescopy_2.js
├── images/                # UI icons and controls
├── js/                    # Leaflet extensions, Autolinker, RBush & Geocoder
├── legend/                # Generated symbology legends
├── markers/               # Map pin graphics
├── index.html             # Main entry point for the interactive WebGIS
├── template layout.qpt    # QGIS Print Layout template
├── membuat layout.qgz     # Master QGIS project archive
└── README.md              # Project documentation
```

---

## ⚙️ Running Locally (Offline)

This export is **100% standalone** and does not require server-side dependencies:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/billiampalad/Peta-Kalimantan.git
   ```
2. **Navigate to the project folder:**
   ```bash
   cd Peta-Kalimantan
   ```
3. **Open the map:**
   - Simply double-click **`index.html`** or open it in your preferred web browser (Google Chrome, Firefox, Microsoft Edge, Safari).
   - Alternatively, serve it via any local development server:
     ```bash
     npx serve .
     ```

---

## 👤 Author & Acknowledgments

- **Author**: Clynten Billiam Palad
- **GitHub**: [@billiampalad](https://github.com/billiampalad)
- **Data Source**: [Natural Earth Public Domain Maps](https://www.naturalearthdata.com/)
- **Software**: The open-source geospatial community & QGIS Project.

<div align="center">
  <sub>Built with ❤️ for GIS Semester 6 • Clynten Billiam Palad</sub>
</div>
