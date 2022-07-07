---
title: "AI4ES data"
---

> See [[AI4ES/AI4ES#Infrastructure and data]]

## Climate data
- [[Climate change#Data and viz]]
- [Climate Data Store - Copernicus](https://cds.climate.copernicus.eu)
	- [CEMS - Emergency Management System](https://emergency.copernicus.eu/)
- https://github.com/pangeo-data/
- [The DL4ES book, DATA](https://github.com/DL4ES/DL4ES)
- [Climate Reanalyzer](https://climatereanalyzer.org/)
	- platform for visualizing climate and weather datasets
- [AWS climate data](https://registry.opendata.aws/tag/climate/)
- [SpatioTemporal Asset Catalogs](https://stacspec.org/)
	- The STAC specification is a common language to describe geospatial information, so it can more easily be worked with, indexed, and discovered.
	- [intake-stac](https://medium.com/pangeo/introducing-intake-stac-2c988d8e1d30)
- [Cryosphere](https://github.com/awesome-cryosphere/cryosphere-links)

- #PAPER [Enabling Immediate Access to Earth Science Models through Cloud Computing: Application to the GEOS-Chem Model (Zhuang 2019)](https://journals.ametsoc.org/bams/article/100/10/1943/344808/Enabling-Immediate-Access-to-Earth-Science-Models)
- #PAPER [A Portal Offering Standard Visualization and Analysis on top of an Open Data Cube for Sub-National Regions: The Catalan Data Cube Example (Maso 2019)](https://www.mdpi.com/2306-5729/4/3/96)
- #PAPER [Seven Principles for Effective Scientific Big-Data Systems (Robinson 2020)](https://arxiv.org/abs/1908.03356)
- #PAPER [Open weather and climate science in the digital era (de Vos 2020)](https://gc.copernicus.org/articles/3/191/2020/)
	- The application of the findable, accessible, interoperable, and reusable (FAIR) principles to many datasets used in weather and climate science remains a challenge
	- This may be due to scalability (in the case of high-resolution climate model data, for example), legal barriers such as those encountered in using weather forecast data, or issues with heterogeneity (for example, when trying to make use of citizen data)
	- There is a need for new roles and responsibilities in the scientific process. People working at the interface of science and digital technology – e.g., data stewards and research software engineers – should collaborate with domain researchers to ensure the optimal use of open science tools and methods
- #PAPER [WeatherBench: A benchmark dataset for data-driven weather forecasting (Rasp 2020)](https://arxiv.org/abs/2002.00469)
	- https://github.com/pangeo-data/WeatherBench
- #PAPER [Comparison of ERA5-Land and UERRA MESCAN-SURFEX Reanalysis Data with Spatially Interpolated Weather Observations for the Regional Assessment of Reference Evapotranspiration (Pelosi 2020)](https://www.mdpi.com/2073-4441/12/6/1669/htm)
- #PAPER [The WGLC global gridded lightning climatology and time series (Kaplan 2021)](https://essd.copernicus.org/articles/13/3219/2021/)
- #POSTER [d-IMERG: A spatiotemporal benchmark dataset for precipitation forecasting (Choi 2022)](https://drive.google.com/file/d/1KEFaebOSNLJJKlCUfsBhgS92gYz6Yd9q/view)
	- The d-IMERG is a subset of images of IMERG providing HDF5 format over four different regions
	- IMERG combines microwave satellite observations from the Global Precipitation Measurement (GPM) satellite constellation to estimate precipitation on a global scale. As microwave measurements can penetrate the precipitating clouds, it provides crucial information on precipitation and clouds. 
- #PAPER [WeatherBench Probability: A benchmark dataset for probabilistic medium-range weather forecasting along with deep learning baseline models (Garg 2022)](https://arxiv.org/pdf/2205.00865)
	- WeatherBench Probability extends WeatherBench to probabilistic forecasting by adding a set of established probabilistic verification metrics (continuous ranked probability score, spread-skill ratio and rank histograms) and a state-of-the-art operational baseline using the ECWMF IFS ensemble forecast

### Projections
- [CIL Global Downscaled Projections for Climate Impacts Research](https://planetarycomputer.microsoft.com/dataset/group/cil-gdpcir)
	- The Global Downscaled Projections for Climate Impacts Research dataset makes this modeling more applicable to understanding the impacts of changes in the climate on humans and society with two key developments: trend-preserving bias correction and downscaling. In this dataset, the Climate Impact Lab provides global, daily minimum and maximum air temperature at the surface (tasmin and tasmax) and daily cumulative surface precipitation (pr) corresponding to the CMIP6 historical, ssp1-2.6, ssp2-4.5, ssp3-7.0, and ssp5-8.5 scenarios for 25 global climate models on a 1/4-degree regular global grid.

### Seasonal forecasts
- [C3S Seasonal forecasts](https://climate.copernicus.eu/seasonal-forecasts)
- #PAPER [SEAS5: the new ECMWF seasonal forecast system (Johnson 2019)](https://gmd.copernicus.org/articles/12/1087/2019/) ^seas5
	- ECMWF's fifth generation seasonal forecast system
	- https://www.ecmwf.int/sites/default/files/medialibrary/2017-10/System5_guide.pdf
	- https://www.ecmwf.int/en/newsletter/154/meteorology/ecmwfs-new-long-range-forecasting-system-seas5

### AC forecasts
- CAMS - Copernicus Atmosphere Monitoring Service: 
	- https://www.ecmwf.int/en/forecasts/dataset/cams-global-atmospheric-composition-forecasts
	- https://atmosphere.copernicus.eu/accessing-atmospheric-composition-forecasts-made-easy
	- https://ads.atmosphere.copernicus.eu/cdsapp#!/dataset/cams-global-atmospheric-composition-forecasts?tab=doc
	- [CAMSRA global reanalysis at 0.8 deg (80x80 km)](https://www.ecmwf.int/en/forecasts/dataset/cams-global-reanalysis)
	- CAMS regional reanalysis at 0.1 deg (10x10 km):
		- https://confluence.ecmwf.int/display/CKB/CAMS+Regional%3A+European+air+quality+analysis+and+forecast+data+documentation
		- https://ads.atmosphere.copernicus.eu/cdsapp#!/dataset/cams-europe-air-quality-forecasts?tab=overview
	- #PAPER [The CAMS reanalysis of atmospheric composition (Inness 2019)](https://acp.copernicus.org/articles/19/3515/2019/)

### Reanalysis
- [ERA5](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview)
	- #PAPER [The ERA5 global reanalysis (Hersbach 2020)](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.3803) ^era5
	- https://www.ecmwf.int/en/forecasts/datasets/reanalysis-datasets/era5
	- ERA5 is an atmospheric reanalysis, so uses ocean and land surface only as boundary condition
	- The data cover the Earth on a 30km grid and resolve the atmosphere using 137 levels from the surface up to a height of 80km
	- ERA5 includes information about uncertainties for all variables at reduced spatial and temporal resolutions
	- ERA5 combines vast amounts of historical observations into global estimates using advanced modelling and data assimilation systems

#### Precipitation
- [Precipitation datasets comparison](https://climatedataguide.ucar.edu/climate-data/precipitation-data-sets-overview-comparison-table)

- #PAPER [MSWEP: 3-hourly 0.25◦global gridded precipitation (1979–2015)by merging gauge, satellite, and reanalysis data (Beck 2017)](https://hess.copernicus.org/preprints/hess-2017-508/hess-2017-508.pdf)
	- http://www.gloh2o.org/mswep/
	- Multi-Source Weighted-Ensemble Precipitation
	- Fully global (including ocean areas) historical precipitation dataset (1979–2019) with a 3‑hourly temporal and 0.1° spatial resolution
	- MSWEP takes advantage of the complementary strengths of gauge‑, satellite‑, and reanalysis-based data to provide reliable precipitation estimates over the entire globe
	- #BSC /esarchive/recon/gloh2o/mswep
	- Global precipitation
- #PAPER [PTHRES. High-Resolution Temperature Datasets in Portugal from a Geostatistical Approach: Variability and Extremes (Fonseca, 2017)](https://journals.ametsoc.org/jamc/article/57/3/627/68273/High-Resolution-Temperature-Datasets-in-Portugal)
- #PAPER [An Ensemble Version of the E-OBS Temperature and Precipitation Data Sets (Cornes 2018)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2017JD028200)
	- https://www.researchgate.net/publication/327013373_An_Ensemble_Version_of_the_E-OBS_Temperature_and_Precipitation_Data_Sets
	- [E-OBS ](https://climatedataguide.ucar.edu/climate-data/e-obs-high-resolution-gridded-meanmaxmin-temperature-precipitation-and-sea-level )
	- daily data with extent: 25N-71.5N x 25W-45E  
	- used for [[Abstract - ENES HPC]]
	- [Southeast Asia version of E-OBS](http://sacad.database.bmkg.go.id/)
- UERRA [[AI4ES/AI4ES data#^uerra]]
- #PAPER [The Global Precipitation Climatology Project (GPCP) Monthly Analysis (New Version 2.3) and a Review of 2017 Global Precipitation (Adler 2018)](https://www.mdpi.com/2073-4433/9/4/138)
	- #BSC /esarchive/obs/nasa/gpcp_v2.2/daily_mean/prlr, /esarchive/obs/nasa/gpcp_v2.3/monthly_mean/prlr
	- https://climatedataguide.ucar.edu/climate-data/gpcp-monthly-global-precipitation-climatology-project
	- Global precipitation
- #PAPER [Iberia01: a new gridded dataset of daily precipitation and temperatures over Iberia (Herrera 2019)](https://essd.copernicus.org/articles/11/1947/2019/)
	- showed that Iberia01 produces more realistic precipitation patterns than E-OBS for the mean and extreme indices considered, although both are comparable for temperatures
- #PAPER [FROGS: a daily 1°  ×  1° gridded precipitation database of rain gauge, satellite and reanalysis products (Roca 2019)](https://essd.copernicus.org/articles/11/1017/2019/  )
	- Global precipitation
- #PAPER [IMERG V06: Changes to the Morphing Algorithm (Tan 2019)](https://journals.ametsoc.org/view/journals/atot/36/12/jtech-d-19-0114.1.xml)
	- https://disc.gsfc.nasa.gov/datasets/GPM_3IMERGHH_06/summary
	- https://gpm.nasa.gov/data/imerg
	- [Global precipitation measurement](https://gpm.nasa.gov/)
	- Global precipitation
- #PAPER [Rainfall Estimates on a Gridded Network (REGEN) – a global land-based gridded dataset of daily precipitation from 1950 to 2016 (Contractor 2020)](https://www.hydrol-earth-syst-sci.net/24/919/2020/)
	- Global precipitation
- #PAPER [RainBench - Towards Global Precipitation Forecasting from Satellite Imagery (Schroeder de Witt 2020)](https://arxiv.org/abs/2012.09670	) ^rainbench
	- [RainBench - Enabling Data-driven precipitation forecasting on a global scale (Tong 2020)](https://www.climatechange.ai/papers/neurips2020/38)
	- Multi-modal benchmark dataset dedicated to advancing global precipitation forecasting
		- SimSat. ECMWF model-simulated satellite data. 3-hourly, 0.1º. Lag time of 24h
		- IMERG. NASA global half-hourly precipitation estimation. The final run product uses satellite data from multiple polar-orbiting and geo-stationary satellites, corrected with reanalysis (MERRA2, ERA5) and rain-gauge data. 0.1º. Lag time of 3-4 months
		- ERA5. Reanalysis, 1-hourly. Including other atmospheric variables (specific humidity, temperature and geopotential height). 0.25º. Lag time 5 days
	- PyRain works with WeatherBench. Based on NumPy memmap arrays
	- ConvLSTMs
	- Mean latitude-weighted Root-Mean Squared Error (RMSE) as loss and evaluation metric

#### Other reanalysis data
- JRA-55 (starts 1958) 
- NCEP1 (starts 1948) -- very old reanalysis (state of art year ~2000) 

### Temperature
- [UERRA regional reanalysis for Europe](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-uerra-europe-single-levels?tab=overview ^uerra)
	- http://www.uerra.eu/component/dpattachments/?task=attachment.download&id=385
	- www.uerra.eu/component/dpattachments/?task=attachment.download&id=399
- [HadCRUT5 - gridded dataset of global historical surface temperature anomalies relative to a 1961-1990 reference period](https://www.metoffice.gov.uk/hadobs/hadcrut5/)

### Soil moisture
- ERA5-Land https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land?tab=overview 
- [GLEAM - Global Land Evaporation Amsterdam Model](https://www.gleam.eu/)
	- different components of land evaporation (often referred to as '_evapotranspiration_’): transpiration, bare-soil evaporation, interception loss, open-water evaporation and sublimation
	- soon to come HR evaporation data
	- products: Soil Evaporation, Snow Sublimation, Transpiration, Open-water Evaporation, Evaporative Stress, Root-zone Soil Moisture, Surface Soil Moisture
	- #PAPER [GLEAM v3: satellite-based land evaporation and root-zone soil moisture (Marterns 2017)](https://gmd.copernicus.org/articles/10/1903/2017/)

### Wind
- #PAPER [What global reanalysis best represents near-surface winds? (Ramon 2019)](https://rmets.onlinelibrary.wiley.com/doi/epdf/10.1002/qj.3616)
	- In an effort to identify the products that best represent the wind speed features at turbine hub heights, five state-of-the-art global reanalyses have been analysed: ERA5,ERA-Interim, the Japanese 55-year Reanalysis (JRA55), the Modern Era Retrospective Analysis for Research and Applications-2 (MERRA2), and the National Centersfor Environmental Prediction (NCEP)/National Center for Atmospheric Research(NCAR) Reanalysis 1 (R1)
	- Comparison with in situ observations shows that the ERA5 surface winds offer the best agreement, correlating and reproducing the observed variability better than a multi-reanalysis mean in 35.1% of the tall tower sites on a daily time-scale.

### Fires
- [MODIS Thermal Anomalies/Fire](https://modis.gsfc.nasa.gov/data/dataprod/mod14.php)
- FireCCI51 and FireCCILT11, ESA Climate Change Initiative
	- https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-3/New_long-term_dataset_to_analyse_global_fire_trends
	- The current focus of the team, led by Emilio Chuvieco from the University of Alcalá in Spain, is to merge data from Copernicus Sentinel-3’s Ocean and Land Colour Instrument (OLCI) and its Sea and Land Surface Temperature Radiometer (SLSTR) into their existing global burned area product, FireCCI51 (2001–19)
- #PAPER [1980–2018 global fire danger re-analysis dataset for the Canadian Fire Weather Indices (Vitolo 2019)](https://www.nature.com/articles/sdata201932)
	- 38 years of global reanalysis of wildfire danger
	- The scientific community is actively studying (through in situ observation and remote sensing) fire behavior to better identify the atmospheric predictors that determine a sustained fire activity once an ignition has occurred
	- It is intuitive that low humidity combined to high temperature tends to dry dead and live fuels which ignite easier than moist fuel
	- Canadian Fire Weather Index (FWI) - is one of the most widely used model to estimate fire danger worldwide
	- The FWI operates by predicting the responses of fuel moisture to atmospheric forcings at different soil depths and by combining these to derive fire behavior indices in terms of ease of spread and intensity
	- The FWI danger rating system was designed to exploit the information provided by in situ observations and it only depends on weather variables
	- The fire danger reanalysis dataset is made of seven gridded fields (or indices) calculated from the Canadian Fire Weather Index model using weather forcings from the ECMWF ERA-Interim reanalysis dataset
	- #CODE https://github.com/esowc/wildfire-forecasting
- [Global Fire Emission Database (GFED4)](http://www.globalfiredata.org)
	- Global Fire Emissions Database version 4 with small fires (GFEDv4s)
- [The CAMS Global Fire Assimilation System (GFAS) ](https://atmosphere.copernicus.eu/global-fire-emissions)
	- GFAS assimilates fire radiative power (FRP) observations from satellite-based sensors to produce daily estimates of wildfire and biomass burning emissions. It also provides information about injection heights derived from fire observations and meteorological information from the operational weather forecasts of ECMWF
	- The GFAS data output includes spatially gridded Fire Radiative Power (FRP), dry matter burnt and biomass burning emissions for a large set of chemical, greenhouse gas and aerosol species
	- Data are available globally on a regular latitude-longitude grid with horizontal resolution of 0.1 degrees from 2003 to present

### Biomass
- [CCI biomass](https://climate.esa.int/en/projects/biomass/)
	- [Data access requirements](https://climate.esa.int/sites/default/files/Biomass%20D1.3%20Data%20Access%20Requirement%20Document%20V1.0.pdf)


## EO and Satellite data
- [Awesome Satellite Imagery Datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [BigEarthNet - A New Large-Scale Sentinel-2 Benchmark Archive](http://bigearth.net/)
	- https://medium.com/radiant-earth-insights/bigearthnet-benchmark-archive-now-available-on-radiant-mlhub-the-open-repository-for-geospatial-d6c5dbe898c4
- [Hyperlabelme](https://ieeexplore.ieee.org/document/8113131/authors#authors )
- [HyRank (hyperspectral dataset)](http://www2.isprs.org/commissions/comm3/wg4/HyRANK.html )
- [Euro Data Cube](https://eurodatacube.com/)
- [AIREO – AI ready EO training datasets](https://eo4society.esa.int/projects/aireo/)
- [Kelvins - ESA's Advanced Concepts Competition Website. Data challenges](https://kelvins.esa.int/  )
- [AVIRIS-NG aerial hyperspectral remote sensing data](https://avirisng.jpl.nasa.gov/dataportal/)
	- The AVRIS-NG data portal includes an unparalleled publicly available **dataset of hyperspectral remote sensing aerial surveys** on multiple continents, including detected large point-source methane emissions (for many campaigns, plus some point-source CO2 emissions)

- #CODE [EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification (Helber 2019)](https://arxiv.org/abs/1709.00029)
	- https://github.com/phelber/eurosat
- #PAPER DIOR (see [[AI4ES/EO]])
- #PAPER [DOTA: A Large-scale Dataset for Object Detection in Aerial Images (Xia 2019)](https://arxiv.org/abs/1711.10398)
- #PAPER [EarthNet2021: A novel large-scale dataset and challenge for forecasting localized climate impacts (Requena-Mesa 2020)](https://arxiv.org/abs/2012.06246v1)
	- https://paperswithcode.com/dataset/earthnet2021?from=n10
- #PAPER FAIR1M (see [[AI4ES/EO]])
- #PAPER [SpaceML: Distributed Open-source Research with Citizen Scientists for the Advancement of Space Technology for NASA (Koul 2021)](https://arxiv.org/abs/2012.10610)

### LULC
- [Dynamic World](https://github.com/google/dynamicworld)
	- #PAPER [Dynamic World, Near real-time global 10 m land use land cover mapping (Brown 2022)](https://www.nature.com/articles/s41597-022-01307-4)
	- Dynamic World V1 is built by training a deep learning model on densely annotated training labels for 9 land cover classes, and is generated using Google Earth Engine and AI Platform
	- Dynamic World is producing land cover probabilities per pixel for the Sentinel-2 1C: Multispectral TOA mission
- [Impact Observatory, Microsoft and ESRI - Land use/cover (LULC)](https://learn-about.impactobservatory.com/maps)
	- Microsoft AI for Earth, Microsoft Planetary Computer (Sentinel-2 data)
	- https://caitlin-kontgis.medium.com/mapping-the-world-in-unprecedented-detail-7c0513205b90
	- https://www.arcgis.com/home/item.html?id=d3da5dd386d140cf93fc9ecbf8da5e31


### Sentinel 5p (TROPOMI)
- https://docs.sentinel-hub.com/api/latest/data/sentinel-5p-l2/
- [NASA ARSET: Introducing TROPOMI - High Resolution NO2 Observations from Space, Part 2/3](https://www.youtube.com/watch?v=-yOInEUJTYM)

### SAR
- POLinSAR - SAR polarimetry and polarimetric interferometry
	- https://www.esa.int/Applications/Observing_the_Earth/POLinSAR_Advances_in_radar_remote_sensing

## Other data
- [Population gridded data](https://www.pbl.nl/en/image/links/hyde)
- [Word pop](https://www.worldpop.org/)
- [GHS-pop](https://ghsl.jrc.ec.europa.eu/download.php?ds=pop)
- [Open Government Building Data](https://ual.sg/project/ogbd/)