# 🗺️ WebGIS Kalimantan Map

An interactive WebGIS project showcasing regional boundaries, provincial administrative borders, and city/population distribution across the island of Kalimantan (Borneo), Indonesia. This map was created and exported using **QGIS** via the **qgis2web** plugin with the **Leaflet** library.

---

## 🌐 Live Website Demo
This WebGIS application is accessible online via the following link:  
🔗 **[https://billiampalad.github.io/Peta-Kalimantan/](https://billiampalad.github.io/Peta-Kalimantan/)**

---

## 📌 Project Information
- **Course**  : Geographic Information Systems (GIS)
- **Project** : Layouting & WebGIS
- **Author**  : Clynten Billiam Palad

---

## 🗂️ Map Features & Layers
1. **Basemap**:
   - Natural Earth Shaded Relief (`NE1_50M_SR_W`)
2. **Administrative Boundary Layer**:
   - Provincial boundaries across Kalimantan (`ne_10m_admin_1_states_provinces`)
3. **Populated Places & Cities Layer**:
   - Major cities in Kalimantan (`ne_10m_populated_places`) categorized by population size (Banjarmasin, Pontianak, Samarinda, Balikpapan, Palangkaraya, Tarakan, Bontang, Singkawang, Sampit, Martapura, etc.)
4. **Interactive Tools**:
   - *Information Popups*: Click or hover over features to view detailed attribute data.
   - *Location Search (Photon Geocoder)*: Quickly search for specific place names.
   - *Measurement Tool (Leaflet Measure)*: Measure distances and calculate areas directly on the map.
   - *Layer Control*: Toggle visibility of specific map layers as needed.

---

## 📁 Data Sources
- **Natural Earth Data**:
  - 1:10m Cultural Vectors (Admin 1 – States, Provinces & Populated Places)
  - 1:50m Raster Data (Natural Earth I with Shaded Relief and Water)

---

## 💻 Running Locally (Offline)
This export is completely standalone:
1. Open this project directory or clone the repository to your computer.
2. Double-click **`index.html`** to open and run the map directly in your web browser (Chrome, Firefox, Edge, etc.).
3. No web server or additional software is required for local viewing.
