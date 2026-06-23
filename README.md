Mali Agricultural Drought Monitoring Dashboard

Project Description

This project develops an agricultural drought monitoring system for Mali by integrating satellite-derived vegetation indicators and rainfall-based drought indices. The dashboard combines rainfall anomalies, Standardized Precipitation Index (SPI), Normalized Difference Vegetation Index (NDVI) anomalies, and Vegetation Condition Index (VCI) to identify drought hotspots across Mali.

The project demonstrates the use of climate and remote sensing data for drought early warning and agricultural monitoring.

Objectives
Monitor rainfall variability across Mali.
Detect meteorological drought using SPI.
Assess vegetation stress using NDVI and VCI.
Identify agricultural drought hotspots by combining SPI and VCI.
Visualize drought conditions through interactive charts and maps.
Datasets Used
Dataset	Source	Period
CHIRPS Rainfall	CHIRPS Climate Data Archive	1981–2026
NDVI	MODIS Vegetation Indices Products or GIMMS NDVI3g Dataset	2002–2026
Administrative Boundaries	Humanitarian Data Exchange (HDX) Mali Boundaries	Current
Methodology
1. Data Cleaning
Removed missing values.
Standardized date formats.
Harmonized administrative units.
Aggregated monthly observations.
2. Rainfall Anomalies

Rainfall anomalies were calculated as:

Anomaly=Rainfall
i
	​

−
Rainfall
	​

3. Standardized Precipitation Index (SPI)

SPI was computed to quantify meteorological drought severity.

Interpretation:

SPI	Category
> 0	Wet conditions
-1 to 0	Mild drought
-1.5 to -1	Moderate drought
-2 to -1.5	Severe drought
< -2	Extreme drought
4. NDVI Anomalies

Vegetation anomalies were computed relative to long-term mean NDVI values.

5. Vegetation Condition Index (VCI)
VCI=
NDVI
max
	​

−NDVI
min
	​

NDVI
i
	​

−NDVI
min
	​

	​

×100

VCI interpretation:

VCI (%)	Condition
0–20	Extreme drought
21–35	Severe drought
36–50	Moderate drought
>50	Normal
6. Agricultural Drought Hotspots

SPI and VCI were combined to classify drought severity.

Example classification:

SPI	VCI	Status
SPI < -1 and VCI < 35	Severe Drought	
SPI < -1 and VCI < 50	Moderate Drought	
SPI < 0 and VCI < 35	Watch	
Otherwise	Normal	
Technologies Used
Python
Pandas
NumPy
GeoPandas
Matplotlib
Plotly
Folium
Jupyter Notebook
GIS (QGIS/ArcGIS)
Repository Structure
Mali_Drought_Monitoring_Dashboard/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_rainfall_anomalies.ipynb
│   ├── 03_spi_calculation.ipynb
│   ├── 04_ndvi_anomalies.ipynb
│   ├── 05_vci_calculation.ipynb
│   └── 06_hotspot_mapping.ipynb
│
├── maps/
├── dashboard/
├── figures/
├── README.md
├── requirements.txt
└── LICENSE
Expected Outputs
Rainfall anomaly time series.
SPI drought analysis.
NDVI anomaly analysis.
VCI maps.
Agricultural drought hotspot maps.
Interactive drought dashboard for Mali.
Key Skills Demonstrated
Climate data analysis
Remote sensing
GIS and spatial analysis
Drought monitoring
Data visualization
Python programming
Environmental data science
Dashboard development

For your LinkedIn and portfolio, this project strongly demonstrates practical expertise in climate analytics, remote sensing, GIS, and agricultural drought monitoring, which are highly valuable in organizations such as World Food Programme, FAO, USAID, and FEWS NET.

---

