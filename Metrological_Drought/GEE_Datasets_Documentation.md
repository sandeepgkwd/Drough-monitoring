# GEE Datasets Used - Gangapur Climate Analysis (1990-2025)

## 1. Temperature

**Dataset 1**: `ECMWF/ERA5_LAND/MONTHLY_AGGR`
- **Available Range**: 1950-present (3 months delay)
- **Used Period**: 1990-2023
- **Type**: Monthly reanalysis data


**Dataset 2**: `MODIS/061/MOD11A2`
- **Available Range**: 2000-present (near real-time)
- **Used Period**: 2024-Sept 2025
- **Type**: 8-day Land Surface Temperature
- **Resolution**: 1 km

## 2. Rainfall

**Dataset**: `UCSB-CHG/CHIRPS/DAILY`
- **Available Range**: 1981-present (near real-time)
- **Used Period**: 1990-Sept 2025
- **Type**: Daily satellite-gauge data
- **Resolution**: ~5.5 km

## 3. Humidity

**Dataset**: `ECMWF/ERA5_LAND/MONTHLY_AGGR`
- **Available Range**: 1950-present (3 months delay)
- **Used Period**: 1990-Sept 2025
- **Type**: Monthly reanalysis data
- **Resolution**: ~11 km
- **Parameter**: Relative humidity from dewpoint temperature

---

# CSV Datasets - Time Series Data

| Parameter | Dataset Name | Period Used |
|-----------|--------------|-------------|
| **Temperature** | ERA5-Land / MODIS LST | 1990-Sept 2025 |
| **Rainfall** | CHIRPS | 1990-Sept 2025 |
| **Humidity** | ERA5-Land | 1990-Sept 2025 |

## 3.2.3.1 ERA5-Land (Temperature and Humidity)
- **Dataset**: `ECMWF/ERA5_LAND/MONTHLY_AGGR`
- **Variables**: Temperature (mean, min, max), Relative Humidity
- **Resolution**: ~11 km
- **Temporal**: Monthly
- **Coverage**: Global

## 3.2.3.2 MODIS LST (Temperature)
- **Dataset**: `MODIS/061/MOD11A2`
- **Variables**: LST_Day_1km, LST_Night_1km
- **Resolution**: 1 km
- **Temporal**: 8-day composite
- **Coverage**: Global

## 3.2.3.3 CHIRPS (Rainfall)
- **Dataset**: `UCSB-CHG/CHIRPS/DAILY`
- **Variables**: Precipitation
- **Resolution**: ~5.5 km
- **Temporal**: Daily
- **Coverage**: Global (50°S-50°N)

---

# TIFF Datasets - Spatial Raster Files

| Parameter | Files | Period | Format | Source |
|-----------|-------|--------|---------|---------|
| **Temperature** | 35 files | 1990-2024 | Gangapur_Temp_YYYY.tif | ERA5-Land / MODIS |
| **Rainfall** | 40 files | 2005-2024 | Rainfall_YYYY_Period.tif | CHIRPS |
| **Humidity** | 34 files | 1990-2023 | Gangapur_RH_YYYY.tif | ERA5-Land |

**File Locations:**
- Temperature: `TIFF Files/GEE_Temperature/`
- Rainfall: `TIFF Files/GEE_Rainfall_/` (6-month splits)
- Humidity: `TIFF Files/GEE_Humidity/`

**Output Visualizations:**
- temp_spatial.png
- rainfall_spatial.png
- humidity_spatial.png
- spatial.pptx (PowerPoint)