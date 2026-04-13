# Phoenix-Neighborhood-Change-Analysis-Geospatial-Dashboard-2000-2010-
Phoenix Neighborhood Change Analysis : Geospatial Dashboard (2000–2010)

Built an end-to-end geospatial analysis and interactive Shiny/flexdashboard exploring neighborhood change across Maricopa County, AZ using census tract data from 2000 and 2010 (LTDB Longitudinal Tract Database).

• Engineered a full R-based data pipeline: loaded U.S. Census tract boundaries via the tigris API, merged with LTDB socioeconomic data across 200+ variables, standardized GEOIDs, and filtered valid tracts producing a clean spatial dataset for downstream analysis.
• Generated a Dorling cartogram (population-weighted bubble map) using the cartogram package, projected to WGS84 and exported as GeoJSON enabling proportional spatial representation of census tracts by population size.
• Built a multi-tab interactive Flexdashboard with Leaflet maps, Plotly charts, and DT tables covering: neighborhood cluster analysis (MClust), median home value change, population shifts, demographic breakdowns (race, education, poverty), and tract-level popups.
• Applied Gaussian mixture model clustering (MClust) to segment Phoenix neighborhoods into distinct types based on demographics, housing, and socioeconomic indicators surfacing spatial patterns of inequality and gentrification.

Tech: R · Leaflet · Shiny · Flexdashboard · Plotly · MClust · cartogram · tigris · sf · GeoJSON · LTDB Census Data
