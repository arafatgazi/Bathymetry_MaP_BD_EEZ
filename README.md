# Bangladesh Exclusive Economic Zone (EEZ) & Coastal Bathymetry (100m Contours)

This repository contains processed bathymetric data, a 100-meter interval contour map, and spatial boundary shapefiles covering the **Exclusive Economic Zone (EEZ) and coastal zone of Bangladesh** (Bay of Bengal). All spatial processing, clipping, and contour generation were performed using **QGIS**.

---

## 📋 Overview & Purpose

* **Study Area:** Bangladesh Exclusive Economic Zone (EEZ) and adjacent coastal waters.
* **Data Type:** Gridded bathymetry raster, 100m bathymetric contour lines, and boundary shapefiles.
* **GIS Software:** QGIS (Open Source Geographic Information System).
* **Use Cases:** Marine spatial planning, oceanography, coastal engineering, fisheries research, and GIS mapping projects in Bangladesh.

---

## 📂 Repository Contents

*(Update the file names below to match the exact files in your folder)*

* `BD_EEZ_Coastal_Boundary.shp` *(+ `.shx`, `.dbf`, `.prj`, `.cpg`)* — Vector shapefile defining the Bangladesh Exclusive Economic Zone and coastal boundary.
* `BD_EEZ_Bathymetry_Clipped.tif` — GEBCO bathymetry raster clipped strictly to the Bangladesh EEZ and coastal extent.
* `BD_Bathymetry_Contours_100m.shp` *(+ `.shx`, `.dbf`, `.prj`, `.cpg`)* — Bathymetric contour lines extracted at **100-meter depth intervals**.
* `Maps/` — Exported map layouts (PNG/PDF) visualizing the bathymetry and 100m depth contours.

---

## 🌍 Data Sources & Attribution

1. **Bathymetry Data:** Downloaded from the **GEBCO (General Bathymetric Chart of the Oceans)** Gridded Bathymetry Data portal ([https://gebco.net](https://gebco.net)).
2. **Maritime & Coastal Boundaries:** Bangladesh EEZ and coastal zone boundary shapefile *(e.g., sourced from Marine Regions / Flanders Marine Institute or local maritime boundary datasets—update if applicable)*.

---

## 🛠️ Processing Workflow (QGIS)

The datasets in this repository were prepared using the following workflow in **QGIS**:

1. **Data Acquisition:** Downloaded the regional bathymetry grid (GeoTIFF/NetCDF) covering the northern Bay of Bengal from GEBCO.
2. **Boundary Preparation:** Loaded the Bangladesh EEZ and coastal zone polygon shapefile and verified the Coordinate Reference System (CRS: `EPSG:4326 - WGS 84`).
3. **Raster Clipping:** Clipped the raw GEBCO bathymetry raster to the Bangladesh EEZ and coastal boundary (`Raster` → `Extraction` → `Clip Raster by Mask Layer`).
4. **Contour Generation:** Extracted bathymetric contour lines at **100 m intervals** from the clipped DEM (`Raster` → `Extraction` → `Contour`, with Interval set to `100.0`).
5. **Symbology & Map Layout:** Styled depth classes using a bathymetric color ramp, labeled major contour intervals, and exported the final map layout via QGIS Print Layout.

---

## 🚀 How to Use

1. **Clone or Download** this repository:https://github.com/arafatgazi/Bathymetry_MaP_BD_EEZ
   ```bash
   git clone 
   ```
2. Open **QGIS** and load the `.shp` or `.tif` files via `Layer` → `Add Layer` → `Add Vector/Raster Layer`.
3. Ensure all supporting shapefile extensions (`.shp`, `.shx`, `.dbf`, `.prj`) remain in the same directory when loading.

---

## 📜 Citation & License

If you use the datasets or shapefiles from this repository in your research, maps, or publications, please credit **GEBCO** for the underlying bathymetry data and reference this repository.

---

### 🔍 Keywords
`Bangladesh EEZ shapefile`, `Bangladesh Exclusive Economic Zone GIS`, `Bay of Bengal bathymetry`, `GEBCO Bangladesh`, `100m bathymetric contour Bangladesh`, `Bangladesh coastal zone shapefile`, `QGIS bathymetry map`
