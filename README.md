# Estimating Growing Season Length Using ERA5-Land and Xclim for a Custom Region of Interest
## Overview
This project performs a detailed analysis of Growing Season Length (GSL) for a user-defined region using daily temperature data from ERA5-Land (2000–2020). Growing Season Length is a widely used agro-climatic indicator that helps understand the number of days per year when temperature conditions support plant growth. GSL is crucial for applications such as agricultural planning, crop suitability assessment, yield forecasting, climate variability studies, and long-term adaptation strategies.

By integrating Google Earth Engine, xarray, and xclim, this workflow demonstrates a scalable, reproducible approach to computing climate indices directly from earth observation data. The analysis showcases how large climate datasets can be efficiently accessed, processed, and translated into actionable environmental insights.

A custom region of interest (ROI) was manually selected using an interactive geemap interface. This approach allows users to design flexible study areas tailored to research needs, without relying on administrative boundaries or official political borders. This ensures the analysis is strictly scientific, non-political, and focused solely on environmental assessment.

## Objectives
1. Retrieve daily 2-meter temperature data from the ERA5-Land dataset.
2. Convert temperature from Kelvin to Celsius.
3. Build an xarray dataset using the xee engine.
4. Compute Growing Season Length (GSL) using Xclim.
5. Visualize spatial variability in GSL over time.

### Spatial variation of Growing Season Length across the selected region of interest (2000–2020).
<img width="1472" height="1190" alt="image" src="https://github.com/user-attachments/assets/bee07183-3d14-466f-97db-ee30df492128" />


## Tools & Libraries
### Primary Python Libraries
| Library        | Purpose                                               |
| -------------- | ----------------------------------------------------- |
| **geemap**     | For interactive ROI selection and GEE integration     |
| **xee**        | For loading Earth Engine ImageCollections into xarray |
| **xarray**     | For multi-dimensional climate data handling           |
| **xclim**      | For computing climate indices such as GSL             |
| **matplotlib** | For plotting and saving output maps                   |

### Data Source
1. ECMWF / ERA5-Land (DAILY_AGGR)
- Variable used: temperature_2m
- Time period: 2000–2020
- Spatial resolution: 0.27°

## Notes
- The ROI is not an official administrative or national boundary.It is a manually selected polygon used purely for scientific and analytical purposes.
- All results are for research, demonstration, and methodological learning, not for policy or boundary interpretation.
- Always ensure that any public visualization follows proper cartographic and ethical mapping guidelines, especially when visualizing regions with sensitive or disputed boundaries.
