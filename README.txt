# 🗺️ WebGIS Peta Kalimantan

Proyek WebGIS interaktif yang menyajikan peta wilayah, batas administratif provinsi, dan persebaran kota/penduduk di Pulau Kalimantan. Peta ini dibuat dan diekspor menggunakan **QGIS** melalui plugin **qgis2web** dengan pustaka **Leaflet**.

---

## 🌐 Akses Website (Live Demo)
Aplikasi WebGIS ini dapat diakses secara langsung secara online melalui tautan berikut:  
🔗 **[https://billiampalad.github.io/Peta-Kalimantan/](https://billiampalad.github.io/Peta-Kalimantan/)**

---

## 📌 Informasi Proyek
- **Mata Kuliah** : Sistem Informasi Geografis
- **Projek**       : Layouting & WebGIS
- **Penyusun**    : Clynten Billiam Palad

---

## 🗂️ Fitur & Layer Peta
1. **Peta Dasar (Basemap)**:
   - Shaded Relief Natural Earth (`NE1_50M_SR_W`)
2. **Layer Administrasi**:
   - Batas wilayah provinsi di Kalimantan (`ne_10m_admin_1_states_provinces`)
3. **Layer Persebaran Penduduk & Kota**:
   - Titik-titik kota di Pulau Kalimantan (`ne_10m_populated_places`) dengan klasifikasi ukuran populasi (Banjarmasin, Pontianak, Samarinda, Balikpapan, Palangkaraya, Tarakan, Bontang, Singkawang, Sampit, Martapura, dll.)
4. **Alat Interaktif**:
   - *Popup Informasi*: Klik atau arahkan kursor ke fitur untuk melihat data atribut detail.
   - *Pencarian Lokasi (Photon Geocoder)*: Pencarian nama lokasi secara cepat.
   - *Pengukuran (Leaflet Measure)*: Pengukuran jarak dan luas area langsung pada peta.
   - *Kontrol Layer*: Mengaktifkan/menonaktifkan layer sesuai kebutuhan.

---

## 📁 Sumber Data
- **Natural Earth Data**:
  - 1:10m Cultural Vectors (Admin 1 – States, Provinces & Populated Places)
  - 1:50m Raster Data (Natural Earth I with Shaded Relief and Water)

---

## 💻 Cara Menjalankan Secara Lokal (Offline)
Ekspor ini bersifat *standalone* (mandiri):
1. Buka folder proyek ekspor atau clone repositori ini ke komputer Anda.
2. Klik dua kali pada file **`index.html`** untuk langsung membuka peta di peramban web (Google Chrome, Firefox, Edge, dll.).
3. Tidak memerlukan web server tambahan untuk pengujian lokal.
