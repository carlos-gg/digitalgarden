---
title: "AI4ES data"
---

> See [[AI4ES/AI4ES#Infrastructure and data]]

## Climate data
- See [[AI4ES/Climate change#Data and visualizations]]
- [Climate Data Store - Copernicus](https://cds.climate.copernicus.eu)
	- [CEMS - Emergency Management System](https://emergency.copernicus.eu/)
		- [Global Flood Awareness System](https://www.globalfloods.eu/technical-information/products/) (GloFAS) - support preparatory measures for flood events worldwide, particularly in large trans-national river basins, by providing: meteorological, seasonal and impact forecasts
- https://github.com/pangeo-data/
- [NOAA gridded climate data](https://psl.noaa.gov/data/gridded/index.html)
- [The DL4ES book, DATA](https://github.com/DL4ES/DL4ES)
- [Climate Reanalyzer](https://climatereanalyzer.org/)
	- platform for visualizing climate and weather datasets
- [AWS climate data](https://registry.opendata.aws/tag/climate/)
- [SpatioTemporal Asset Catalogs](https://stacspec.org/)
	- The STAC specification is a common language to describe geospatial information, so it can more easily be worked with, indexed, and discovered.
	- [intake-stac](https://medium.com/pangeo/introducing-intake-stac-2c988d8e1d30)
- [Cryosphere](https://github.com/awesome-cryosphere/cryosphere-links)
- [PANGEA](https://www.pangaea.de/) - Data Publisher for Earth & Environmental Science
- Regridding:
	- [Regridding Overview (NCAR)](https://climatedataguide.ucar.edu/climate-tools/regridding-overview)
	- [Regridding with CDO](https://www.climate-cryosphere.org/wiki/index.php?title=Regridding_with_CDO)
	- [CDO, horizontal grids](https://code.mpimet.mpg.de/projects/cdo/embedded/index.html#x1-280001.5)

- #PAPER [Enabling Immediate Access to Earth Science Models through Cloud Computing: Application to the GEOS-Chem Model (Zhuang 2019)](https://journals.ametsoc.org/bams/article/100/10/1943/344808/Enabling-Immediate-Access-to-Earth-Science-Models)
- #PAPER [A Portal Offering Standard Visualization and Analysis on top of an Open Data Cube for Sub-National Regions: The Catalan Data Cube Example (Maso 2019)](https://www.mdpi.com/2306-5729/4/3/96)
- #PAPER [Seven Principles for Effective Scientific Big-Data Systems (Robinson 2020)](https://arxiv.org/abs/1908.03356)
- #PAPER [Open weather and climate science in the digital era (de Vos 2020)](https://gc.copernicus.org/articles/3/191/2020/)
	- The application of the findable, accessible, interoperable, and reusable (FAIR) principles to many datasets used in weather and climate science remains a challenge
	- This may be due to scalability (in the case of high-resolution climate model data, for example), legal barriers such as those encountered in using weather forecast data, or issues with heterogeneity (for example, when trying to make use of citizen data)
	- There is a need for new roles and responsibilities in the scientific process. People working at the interface of science and digital technology – e.g., data stewards and research software engineers – should collaborate with domain researchers to ensure the optimal use of open science tools and methods
- #PAPER [The WGLC global gridded lightning climatology and time series (Kaplan 2021)](https://essd.copernicus.org/articles/13/3219/2021/)

### Benchmark datasets
- See METER-ML in [[AI4ES/AC, AQ#Methane emission sources]]
- [Eumetnet postprocessing benchmark dataset](https://github.com/EUPP-benchmark/climetlab-eumetnet-postprocessing-benchmark)
- #PAPER [WeatherBench: A benchmark dataset for data-driven weather forecasting (Rasp 2020)](https://arxiv.org/abs/2002.00469)
	- https://github.com/pangeo-data/WeatherBench
- #PAPER [RainBench - Towards Global Precipitation Forecasting from Satellite Imagery (Schroeder de Witt 2020)](https://arxiv.org/abs/2012.09670	) 
	- [RainBench - Enabling Data-driven precipitation forecasting on a global scale (Tong 2020)](https://www.climatechange.ai/papers/neurips2020/38)
	- Multi-modal benchmark dataset dedicated to advancing global precipitation forecasting
		- SimSat. ECMWF model-simulated satellite data. 3-hourly, 0.1º. Lag time of 24h
		- IMERG. NASA global half-hourly precipitation estimation. The final run product uses satellite data from multiple polar-orbiting and geo-stationary satellites, corrected with reanalysis (MERRA2, ERA5) and rain-gauge data. 0.1º. Lag time of 3-4 months
		- ERA5. Reanalysis, 1-hourly. Including other atmospheric variables (specific humidity, temperature and geopotential height). 0.25º. Lag time 5 days
	- PyRain works with WeatherBench. Based on NumPy memmap arrays
	- ConvLSTMs
	- Mean latitude-weighted Root-Mean Squared Error (RMSE) as loss and evaluation metric
- #POSTER [d-IMERG: A spatiotemporal benchmark dataset for precipitation forecasting (Choi 2022)](https://drive.google.com/file/d/1KEFaebOSNLJJKlCUfsBhgS92gYz6Yd9q/view)
	- The d-IMERG is a subset of images of IMERG providing HDF5 format over four different regions
	- IMERG combines microwave satellite observations from the Global Precipitation Measurement (GPM) satellite constellation to estimate precipitation on a global scale. As microwave measurements can penetrate the precipitating clouds, it provides crucial information on precipitation and clouds. 
- #PAPER [WeatherBench Probability: A benchmark dataset for probabilistic medium-range weather forecasting along with deep learning baseline models (Garg 2022)](https://arxiv.org/pdf/2205.00865)
	- WeatherBench Probability extends WeatherBench to probabilistic forecasting by adding a set of established probabilistic verification metrics (continuous ranked probability score, spread-skill ratio and rank histograms) and a state-of-the-art operational baseline using the ECWMF IFS ensemble forecast
- #PAPER #REVIEW [Challenges and Benchmark Datasets for Machine Learning in the Atmospheric Sciences: Definition, Status, and Outlook (Dueben 2022)](https://journals.ametsoc.org/view/journals/aies/1/3/AIES-D-21-0002.1.xml)

#### Extreme events labeled data
See [[AI4ES/Extremes events#Databases]]
- #PAPER [MPING: Crowd-Sourcing Weather Reports for Research (Elmore 2014)](https://journals.ametsoc.org/bams/article/95/9/1335/87658/MPING-Crowd-Sourcing-Weather-Reports-for-Research)
- #PAPER [ExtremeWeather - A large-scale climate dataset for semi-supervised detection, localization, and understanding of extreme weather events (Racah 2017)](https://arxiv.org/abs/1612.02095)
	- https://extremeweatherdataset.github.io/ 
	- https://papers.nips.cc/paper/6932-extremeweather-a-large-scale-climate-dataset-for-semi-supervised-detection-localization-and-understanding-of-extreme-weather-events
- #PAPER [A High-Resolution Global Gridded Historical Dataset of Climate Extreme Indices (Mistry, 2019)](https://www.mdpi.com/2306-5729/4/1/41/htm)
- #PAPER [ClimateNet: an expert-labelled open dataset and Deep Learning architecture for enabling high-precision analyses of extreme weather (Prabhat 2020)](https://gmd.copernicus.org/preprints/gmd-2020-72/) 
	- https://portal.nersc.gov/project/ClimateNet/ 
	- #CODE https://github.com/andregraubner/ClimateNet
	- ClimateNet – an open, community-sourced human expert-labeled curated dataset – that captures tropical cyclones (TCs) and atmospheric rivers (ARs) in high-resolution climate model output from a simulation of a recent historical period
	- The key contribution of this work is that it paves the way for DL-based automated, hi-fidelity and highly precise analytics of climate data using a curated expert-labelled dataset – ClimateNet
	- https://cs.lbl.gov/news-media/news/2019/climatenet-aims-to-improve-machine-learning-applications-in-climate-science-on-a-global-scale/ 
	- https://www.nersc.gov/research-and-development/data-analytics/big-data-center/climatenet/ 
	- https://eos.org/articles/teaching-machines-to-detect-climate-extremes#.XuxgZhBVnts.twitter
- #PAPER [Deepti: Deep-Learning-Based Tropical Cyclone Intensity Estimation System (Maskey 2020)](https://ieeexplore.ieee.org/document/9149719)
	- http://registry.mlhub.earth/10.34911/rdnt.xs53up/

### Projections
- [CMIP6](https://pcmdi.llnl.gov/CMIP6/)
	- Coupled Model Intercomparison Project Phase 6
- [CIL Global Downscaled Projections for Climate Impacts Research](https://planetarycomputer.microsoft.com/dataset/group/cil-gdpcir)
	- The Global Downscaled Projections for Climate Impacts Research dataset makes this modeling more applicable to understanding the impacts of changes in the climate on humans and society with two key developments: trend-preserving bias correction and downscaling. In this dataset, the Climate Impact Lab provides global, daily minimum and maximum air temperature at the surface (tasmin and tasmax) and daily cumulative surface precipitation (pr) corresponding to the CMIP6 historical, ssp1-2.6, ssp2-4.5, ssp3-7.0, and ssp5-8.5 scenarios for 25 global climate models on a 1/4-degree regular global grid.

### Seasonal forecasts
- [C3S Seasonal forecasts](https://climate.copernicus.eu/seasonal-forecasts)
- #PAPER [SEAS5: the new ECMWF seasonal forecast system (Johnson 2019)](https://gmd.copernicus.org/articles/12/1087/2019/) ^seas5
	- ECMWF's fifth generation seasonal forecast system
	- https://www.ecmwf.int/sites/default/files/medialibrary/2017-10/System5_guide.pdf
	- https://www.ecmwf.int/en/newsletter/154/meteorology/ecmwfs-new-long-range-forecasting-system-seas5

### AC forecasts
- [CAMS](https://ads.atmosphere.copernicus.eu/cdsapp#!/dataset/cams-global-atmospheric-composition-forecasts?tab=doc) - Copernicus Atmosphere Monitoring Service
	- https://www.ecmwf.int/en/forecasts/dataset/cams-global-atmospheric-composition-forecasts
	- https://atmosphere.copernicus.eu/accessing-atmospheric-composition-forecasts-made-easy
	- [CAMSRA global reanalysis at 0.8 deg (80x80 km)](https://www.ecmwf.int/en/forecasts/dataset/cams-global-reanalysis)
	- CAMS regional reanalysis at 0.1 deg (10x10 km):
		- https://confluence.ecmwf.int/display/CKB/CAMS+Regional%3A+European+air+quality+analysis+and+forecast+data+documentation
		- https://ads.atmosphere.copernicus.eu/cdsapp#!/dataset/cams-europe-air-quality-forecasts?tab=overview
	- #PAPER [The CAMS reanalysis of atmospheric composition (Inness 2019)](https://acp.copernicus.org/articles/19/3515/2019/)
	- #PAPER [Comprehensive evaluation of the Copernicus Atmosphere Monitoring Service (CAMS) reanalysis against independent observations: Reactive gases (Wagner 2021)](https://online.ucpress.edu/elementa/article/9/1/00171/117164/Comprehensive-evaluation-of-the-Copernicus)

### Reanalysis 
- [Advancing Reanalysis](https://reanalyses.org/ "Home")
- #PAPER [Comparison of ERA5-Land and UERRA MESCAN-SURFEX Reanalysis Data with Spatially Interpolated Weather Observations for the Regional Assessment of Reference Evapotranspiration (Pelosi 2020)](https://www.mdpi.com/2073-4441/12/6/1669/htm)
- #PAPER [The ERA5 global reanalysis (Hersbach 2020)](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.3803) 
	- [ERA5](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview)
	- https://www.ecmwf.int/en/forecasts/datasets/reanalysis-datasets/era5
	- ERA5 is an atmospheric reanalysis, so uses ocean and land surface only as boundary condition
	- The data cover the Earth on a 30km grid and resolve the atmosphere using 137 levels from the surface up to a height of 80km
	- ERA5 includes information about uncertainties for all variables at reduced spatial and temporal resolutions
	- ERA5 combines vast amounts of historical observations into global estimates using advanced modelling and data assimilation systems
- #PAPER [ERA5-Land: a state-of-the-art global reanalysis dataset for land applications (Muñoz-Sabater 2021)](https://essd.copernicus.org/articles/13/4349/2021/)
	- [ERA5 land](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land?tab=overview)
	- ERA5-Land is a reanalysis dataset providing a consistent view of the evolution of land variables over several decades at an enhanced resolution (0.1 degrees) compared to ERA5
- #PAPER [ERA-20C: An Atmospheric Reanalysis of the Twentieth Century (Poli 2016)](https://journals.ametsoc.org/view/journals/clim/29/11/jcli-d-15-0556.1.xml?tab_body=fulltext-display)
	- ERA-20C is ECMWF's first atmospheric reanalysis of the 20th century, from 1900-2010
	- The horizontal resolution is approximately 125 km. The temporal resolution of the daily products is usually 3-hourly
- [gridMET](https://www.climatologylab.org/gridmet.html)
	- gridMET is a dataset of daily high-spatial resolution (~4-km, 1/24th degree) surface meteorological data covering the contiguous US from 1979-yesterday
- [UERRA](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-uerra-europe-single-levels?tab=overview) regional reanalysis for Europe
	- http://www.uerra.eu/component/dpattachments/?task=attachment.download&id=385
	- www.uerra.eu/component/dpattachments/?task=attachment.download&id=399
- [JRA-55](https://climatedataguide.ucar.edu/climate-data/jra-55)
	- Spanning 1958-present, JRA-55 is the longest third-generation reanalysis that uses the full observing system

### Precipitation
- [Precipitation datasets comparison](https://climatedataguide.ucar.edu/climate-data/precipitation-data-sets-overview-comparison-table)
- See UERRA, ERA5 and ERA5-land reanalyses 
- #PAPER [Evaluation of Gridded Precipitation Data Products for Hydrological Applications in Complex Topography (Gampe 2017)](https://www.mdpi.com/2306-5338/4/4/53)
- #PAPER [PTHRES. High-Resolution Temperature Datasets in Portugal from a Geostatistical Approach: Variability and Extremes (Fonseca, 2017)](https://journals.ametsoc.org/jamc/article/57/3/627/68273/High-Resolution-Temperature-Datasets-in-Portugal)
- #PAPER [An Ensemble Version of the E-OBS Temperature and Precipitation Data Sets (Cornes 2018)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2017JD028200)
	- [E-OBS ](https://climatedataguide.ucar.edu/climate-data/e-obs-high-resolution-gridded-meanmaxmin-temperature-precipitation-and-sea-level )
	- daily data with extent: 25N-71.5N x 25W-45E  
	- [Southeast Asia version of E-OBS](http://sacad.database.bmkg.go.id/)
- #PAPER [The Global Precipitation Climatology Project (GPCP) Monthly Analysis (New Version 2.3) and a Review of 2017 Global Precipitation (Adler 2018)](https://www.mdpi.com/2073-4433/9/4/138)
	- https://climatedataguide.ucar.edu/climate-data/gpcp-monthly-global-precipitation-climatology-project
- #PAPER [Iberia01: a new gridded dataset of daily precipitation and temperatures over Iberia (Herrera 2019)](https://essd.copernicus.org/articles/11/1947/2019/)
	- showed that Iberia01 produces more realistic precipitation patterns than E-OBS for the mean and extreme indices considered, although both are comparable for temperatures
- #PAPER [FROGS: a daily 1°  ×  1° gridded precipitation database of rain gauge, satellite and reanalysis products (Roca 2019)](https://essd.copernicus.org/articles/11/1017/2019/  )
	- Global precipitation
- #PAPER [IMERG V06: Changes to the Morphing Algorithm (Tan 2019)](https://journals.ametsoc.org/view/journals/atot/36/12/jtech-d-19-0114.1.xml)
	- https://disc.gsfc.nasa.gov/datasets/GPM_3IMERGHH_06/summary
	- https://gpm.nasa.gov/data/imerg
	- [Global precipitation measurement](https://gpm.nasa.gov/)
	- Global precipitation
- #PAPER [MSWEP V2 Global 3-Hourly 0.1° Precipitation: Methodology and Quantitative Assessment (Beck 2019)](https://journals.ametsoc.org/view/journals/bams/100/3/bams-d-17-0138.1.xml)
	- Old paper: [MSWEP: 3-hourly 0.25◦global gridded precipitation (1979–2015)by merging gauge, satellite, and reanalysis data (Beck 2017)](https://hess.copernicus.org/preprints/hess-2017-508/hess-2017-508.pdf)
	- http://www.gloh2o.org/mswep/
	- Multi-Source Weighted-Ensemble Precipitation
	- Fully global (including ocean areas) historical precipitation dataset (1979–2019) with a 3‑hourly temporal and 0.1° spatial resolution
	- MSWEP takes advantage of the complementary strengths of gauge‑, satellite‑, and reanalysis-based data to provide reliable precipitation estimates over the entire globe
- #PAPER [Rainfall Estimates on a Gridded Network (REGEN) – a global land-based gridded dataset of daily precipitation from 1950 to 2016 (Contractor 2020)](https://www.hydrol-earth-syst-sci.net/24/919/2020/)
	- Global precipitation
- #PAPER [Comprehensive Comparisons of State-of-the-Art Gridded Precipitation Estimates for Hydrological Applications over Southern China (GAO 2020)](https://www.mdpi.com/2072-4292/12/23/3997?type=check_update&version=3)

### Temperature
- See UERRA and ERA5-land reanalyses
- [HadCRUT5 - gridded dataset of global historical surface temperature anomalies relative to a 1961-1990 reference period](https://www.metoffice.gov.uk/hadobs/hadcrut5/)

### Soil moisture
- See ERA5-Land reanalysis
- #PAPER [GLEAM v3: satellite-based land evaporation and root-zone soil moisture (Marterns 2017)](https://gmd.copernicus.org/articles/10/1903/2017/)
	- [GLEAM - Global Land Evaporation Amsterdam Model](https://www.gleam.eu/)
	- different components of land evaporation (often referred to as '_evapotranspiration_’): transpiration, bare-soil evaporation, interception loss, open-water evaporation and sublimation
	- soon to come HR evaporation data
	- products: Soil Evaporation, Snow Sublimation, Transpiration, Open-water Evaporation, Evaporative Stress, Root-zone Soil Moisture, Surface Soil Moisture

### Wind
- #PAPER [The Global Wind Atlas: An EUDP project carried out by DTU Wind Energy (Badger 2015)](https://backend.orbit.dtu.dk/ws/files/238494910/url.pdf)
	- https://globalwindatlas.info/es/
- #PAPER [Assessing the Global Wind Atlas and local measurements for bias correction of wind power generation simulated from MERRA-2 in Brazil (Gruber 2019)](https://arxiv.org/abs/1904.13083)
- #PAPER [What global reanalysis best represents near-surface winds? (Ramon 2019)](https://rmets.onlinelibrary.wiley.com/doi/epdf/10.1002/qj.3616)
	- In an effort to identify the products that best represent the wind speed features at turbine hub heights, five state-of-the-art global reanalyses have been analysed: ERA5,ERA-Interim, the Japanese 55-year Reanalysis (JRA55), the Modern Era Retrospective Analysis for Research and Applications-2 (MERRA2), and the National Centersfor Environmental Prediction (NCEP)/National Center for Atmospheric Research(NCAR) Reanalysis 1 (R1)
	- Comparison with in situ observations shows that the ERA5 surface winds offer the best agreement, correlating and reproducing the observed variability better than a multi-reanalysis mean in 35.1% of the tall tower sites on a daily time-scale.
- #PAPER [The making of the New European Wind Atlas – Part 1: Model sensitivity (Hahmann 2020)](https://gmd.copernicus.org/articles/13/5053/2020/)
- #PAPER [The Making of the New European Wind Atlas – Part 2: Production and evaluation (Dorenkamper 2020)](https://gmd.copernicus.org/articles/13/5079/2020/)
	- [New European Wind Atlas](https://map.neweuropeanwindatlas.eu/)
		- EU plus Turkey and 100 km offshore as well as the complete North and Baltic Seas
		- The WRF model was used in a NEWA consortium developed configuration
		- 3 km grid spacing and simulation period covering 30 years (1989-2018)
		- Microscale Atlas: https://wps.neweuropeanwindatlas.eu/api/microscale-atlas/v1/docs
		- Mesoscale Atlas: https://wps.neweuropeanwindatlas.eu/api/mesoscale-atlas/v1/docs
- #PAPER [A collection and categorization of open-source wind and wind power datasets (Effenberger 2022)](https://onlinelibrary.wiley.com/doi/10.1002/we.2766)
- #PAPER [Online Wind-Atlas Databases and GIS Tool Integration for Wind Resource Assessment: A Spanish Case Study (Sanchez del Rey 2022)](https://www.mdpi.com/1996-1073/15/3/852)

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
- [ESA openEO Platform](https://openeo.cloud/)
	- openEO platform provides intuitive programming libraries to process a wide variety of earth observation datasets. This large-scale data access and processing is performed on multiple infrastructures, which all support the openEO API
- [Awesome Satellite Imagery Datasets](https://github.com/chrieke/awesome-satellite-imagery-datasets)
- [Hyperlabelme](https://ieeexplore.ieee.org/document/8113131/authors#authors )
- [HyRank (hyperspectral dataset)](http://www2.isprs.org/commissions/comm3/wg4/HyRANK.html )
- [Euro Data Cube](https://eurodatacube.com/)
- [AIREO – AI ready EO training datasets](https://eo4society.esa.int/projects/aireo/)
- [Kelvins - ESA's Advanced Concepts Competition Website. Data challenges](https://kelvins.esa.int/  )
- [AVIRIS-NG aerial hyperspectral remote sensing data](https://avirisng.jpl.nasa.gov/dataportal/)
	- The AVRIS-NG data portal includes an unparalleled publicly available dataset of hyperspectral remote sensing aerial surveys on multiple continents, including detected large point-source methane emissions (for many campaigns, plus some point-source CO2 emissions)
- [CaFFe](https://doi.pangaea.de/10.1594/PANGAEA.940950) (CAlving Fronts and where to Find thEm: a benchmark dataset and methodology for automatic glacier calving front extraction from sar imagery)

### Benchmark datasets
- #PAPER [EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification (Helber 2019)](https://arxiv.org/abs/1709.00029)
	- https://github.com/phelber/eurosat
- #PAPER [Object Detection in Optical Remote Sensing Images: A Survey and A New Benchmark (Li 2019)](https://arxiv.org/abs/1909.00133) 
- #PAPER [DOTA: A Large-scale Dataset for Object Detection in Aerial Images (Xia 2019)](https://arxiv.org/abs/1711.10398)
- #PAPER [EarthNet2021: A novel large-scale dataset and challenge for forecasting localized climate impacts (Requena-Mesa 2020)](https://arxiv.org/abs/2012.06246v1)
	- https://www.earthnet.tech/docs/ds-download/
- #PAPER [FAIR1M: A Benchmark Dataset for Fine-grained Object Recognition in High-Resolution Remote Sensing Imagery (Sun 2021)](https://arxiv.org/abs/2103.05569) 
- #PAPER [SpaceML: Distributed Open-source Research with Citizen Scientists for the Advancement of Space Technology for NASA (Koul 2021)](https://arxiv.org/abs/2012.10610)
- #PAPER [BigEarthNet-MM: A Large Scale Multi-Modal Multi-Label Benchmark Archive for Remote Sensing Image Classification and Retrieval (Sumbul 2021)](https://arxiv.org/pdf/2105.07921)
	- [BigEarthNet - A New Large-Scale Sentinel-2 Benchmark Archive](http://bigearth.net/)
	- [BigEarthNet Benchmark Archive Now Available on Radiant MLHub](https://medium.com/radiant-earth-insights/bigearthnet-benchmark-archive-now-available-on-radiant-mlhub-the-open-repository-for-geospatial-d6c5dbe898c4), the Open Repository for Geospatial Training Data
- #PAPER [Open High-Resolution Satellite Imagery: The WorldStrat Dataset -- With Application to Super-Resolution (Cornebise 2022)](https://arxiv.org/pdf/2207.06418v1)
	- https://github.com/worldstrat/worldstrat
	- Nearly 10,000 km² of free high-resolution satellite imagery of unique locations which ensure stratified representation of all types of land-use across the world: from agriculture to ice caps, from forests to multiple urbanization densities
	- Each high-resolution image (1.5 m/pixel) comes with multiple temporally-matched low-resolution images from the freely accessible lower-resolution Sentinel-2 satellites (10 m/pixel)
	- See [[AI/Computer Vision/Super-resolution]]
- #PAPER [Current Trends in Deep Learning for Earth Observation: An Open-source Benchmark Arena for Image Classification (Dimitrovski 2022)](https://arxiv.org/pdf/2207.07189)
	- AiTLAS: Benchmark Arena -- an open-source benchmark framework for evaluating state-of-the-art deep learning approaches for image classification in Earth Observation
	- #CODE https://github.com/biasvariancelabs/aitlas-arena

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

## Other datasets
- [Population gridded data](https://www.pbl.nl/en/image/links/hyde)
- [Word pop](https://www.worldpop.org/)
- [GHS-pop](https://ghsl.jrc.ec.europa.eu/download.php?ds=pop)
- [Open Government Building Data](https://ual.sg/project/ogbd/)
- [Urban Atlas (Copernicus - Land monitoring service)](https://land.copernicus.eu/local/urban-atlas)
