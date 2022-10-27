---
title: "Atmospheric composition and air quality (AC, AQ)"
---

> See [[AI4ES/Climate change]]

## Resources
- [Atmospheric composition data products](https://iasi.aeris-data.fr/)
- [Chemical transport model (CTM)](https://en.wikipedia.org/wiki/Chemical_transport_model)
	- type of computer numerical model which typically simulates atmospheric chemistry and may give air pollution forecasting
	- CTM focuses on the stocks and flows of one or more chemical species
	- CTM is expected to accurately represent the entire cycle for the species of interest, including fluxes (e.g. advection), chemical production/loss, and deposition
- [Air Quality e-Reporting](https://www.eea.europa.eu/data-and-maps/data/aqereporting-9)
- AI4EO Air quality challenge. See [[AI4G/Challenges in EO and Climate]]

### Methane emissions
- [The MEthane Tracking Emissions Reference (METER) database](https://meterplatform.web.app/)
	- The METER database combines public data set aggregation, crowdsourcing, and artificial intelligence to create a freely available, global repository of methane-emitting infrastructure
- [GHGsat](https://www.bloomberg.com/news/articles/2021-02-12/new-climate-satellite-spotted-giant-methane-leak-as-it-happened)
- Methane tracker: 
	- https://www.iea.org/articles/global-methane-emissions-from-oil-and-gas
	- https://www.iea.org/articles/methane-tracker-database
	- [Mapping methane emissions on a global scale](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-5P/Mapping_methane_emissions_on_a_global_scale)
	- [Monitoring methane emissions from gas pipelines](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-5P/Monitoring_methane_emissions_from_gas_pipelines)

### CO2 emissions
- [Electricity Maps](https://github.com/electricitymaps) - Mapping the carbon footprint of electricity worldwide
	- [Visualización del impacto climático de la electricidad](https://app.electricitymaps.com/map)
	- https://www.genbeta.com/web/este-mapa-interactivo-nos-dice-donde-procede-electricidad-que-se-consume-cada-pais-sus-emisiones-co2
- [Gaussian process regression (GPR) on Mauna Loa CO2 data. — scikit-learn 0.21.3 documentation](https://scikit-learn.org/stable/auto_examples/gaussian_process/plot_gpr_co2.html)


## References
- #PAPER [Forecasting CO2 Emission with Machine Learning Methods (Garip 2018)](https://ieeexplore.ieee.org/document/8620767)
	- https://www.researchgate.net/publication/331426320_Forecasting_CO2_Emission_with_Machine_Learning_Methods
- #PAPER [Forecasting CO2 Emissions from Energy, Manufacturing and Transport Sectors in Pakistan: Statistical Vs. Machine Learning Methods (Ur Rehman 2018)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3292279 )
- #PAPER [A novel method for carbon dioxide emission forecasting based on improved Gaussian processes regression (Fang 2018)](https://www.sciencedirect.com/science/article/abs/pii/S0959652617310429)
- #PAPER [A Neural Attention Model for Urban Air Quality Inference: Learning the Weights of Monitoring Stations (Cheng, 2018)](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16607)
	- Existing approaches to inferring spatially fine-grained air quality information mainly fall into two categories:physical methods and data-driven approaches
	- Proposed a generic neural attention model based on deep neural networks for urban air quality inference. We leverage both records from monitoring stations and various urban data (e.g., meteorology, road networks, POIs), and extract important features that are correlated with air quality
- #THESIS/MSC [Mid-term air quality forecasts using remote sensing data and machine learning (van Linschoten, 2017)](https://staff.fnwi.uva.nl/a.s.z.belloum/MSctheses/MScthesis_Boris_van_linschoten.pdf)
- #PAPER [Estimation of ground-level particulate matter concentrations through the synergistic use of satellite observations and process-based models over South Korea (Park 2019)](https://www.atmos-chem-phys.net/19/1097/2019/)
- #PAPER [Air Quality Forecast through Integrated Data Assimilation and Machine Learning (Lin 2019)](https://www.researchgate.net/publication/330451387_Air_Quality_Forecast_through_Integrated_Data_Assimilation_and_Machine_Learning)
- #PAPER [Machine learning for Inferring CO2 Fluxes: The New Metaphysics of Neural Nets (Nguyen 2019)](https://eartharxiv.org/284f5/)
- #PAPER [California’s methane super-emitters (Duren 2019)](https://www.nature.com/articles/s41586-019-1720-3)
	- Identifying point sources of emissions with HiRes EO. No ML though
- #PAPER [Machine learning for observation bias correction with application to dust storm data assimilation (Jin 2019)](https://www.atmos-chem-phys.net/19/10009/2019/)
	- Two methods have been implemented to remove the non-dust part of the PM10 observations during the dust event in order to use them as a dust proxy in a dust assimilation system
	- The first method uses a conventional regional chemistry transport model, LOTOS-EUROS/non-dust, which simulates the emission, transport, chemistry, and deposition of aerosols mainly related to anthropogenic activities
	- The second method uses a machine learning model (LSTM) that statistically describes the relations between regular PM10 concentrations (outside dust events) and available air quality and meteorological data
	- The best results are obtained when using a LSTM model to remove the non-dust part of the PM10 observations, with a posteriori concentrations in good agreement with the measurements
- #PAPER [MapLUR: Exploring a New Paradigm for Estimating Air Pollution Using Deep Learning on Map Images (Steininger 2020)](https://dl.acm.org/doi/fullHtml/10.1145/3380973)
	- https://arxiv.org/pdf/2002.07493.pdf
- #PAPER [A scientific algorithm to simultaneously retrieve carbon monoxide and methane from TROPOMI onboard Sentinel-5 Precursor (Schneising 2019)](https://www.researchgate.net/publication/333785409)
- #PAPER [TROPOMI NO2 Tropospheric Column Data: Regridding to 1 km Grid-Resolution and Assessment of their Consistency with In Situ Surface Observations (Cersosimo 2020)](https://www.mdpi.com/2072-4292/12/14/2212/htm)
	- Kriging
- #PAPER [Copernicus Atmosphere Monitoring Service TEMPOral profiles (CAMS-TEMPO): global and European emission temporal profile maps for atmospheric chemistry modelling (Guevara 2020)](https://essd.copernicus.org/articles/13/367/2021/)
- #PAPER [Comparison of Machine Learning and Land Use Regression for fine scale spatiotemporal estimation of ambient air pollution: Modeling ozone concentrations across the contiguous United States (Ren 2020)](https://www.sciencedirect.com/science/article/pii/S0160412020317827#bb0130)
- #PAPER [Importance of satellite observations for high-resolution mapping of near-surface NO2 by machine learning (Kim 2021)](https://www.sciencedirect.com/science/article/pii/S0034425721002935#f0035)
	- https://www.empa.ch/web/s503/maps-of-air-pollutants
	- XGBoost per grid-point
	- 100 m resolution
- #PAPER [Exploring Deep Learning for Air Pollutant Emission Estimation (Huang 2021)](https://gmd.copernicus.org/preprints/gmd-2021-80/)
	- #CODE https://zenodo.org/record/4607127#.YGTqgnX7RtM
- #PAPER [The UrbEm Hybrid Method to Derive High-Resolution Emissions for City-Scale Air Quality Modeling (Ramacher 2021)](https://www.mdpi.com/2073-4433/12/11/1404/htm)
	- See [[AI4ES/Statistical downscaling]]
	- non ML but the methodology is useful
	- In addition to a better spatial representation of emission sources and especially hotspots, the air quality modeling results show that UrbEm outputs, when compared to a uniform spatial disaggregation, have an impact on NO2 predictions up to 70% for urban regions with complex topographies, which corresponds to a big improvement of model accuracy (FAC2 > 0.5), especially at the source-impacted sites 
- #PAPER [Near-real-time global gridded daily CO2 emissions (Dou 2021)](<https://www.cell.com/the-innovation/fulltext/S2666-6758(21)00107-7>)
	- https://carbonmonitor-graced.com/
- #PAPER [Physics-informed deep learning for prediction of CO2 storage site response (Shokouhi 2021)](https://www.sciencedirect.com/science/article/abs/pii/S0169772221000747)
- #PAPER [Importance of satellite observations for high-resolution mapping of near-surface NO2 by machine learning (Kim 2021)](https://www.sciencedirect.com/science/article/pii/S0034425721002935)
- #PAPER [MethaNet – An AI-driven approach to quantifying methane point-source emission from high-resolution 2-D plume imagery (Jongaramrungruang 2022)](https://www.sciencedirect.com/science/article/abs/pii/S0034425721005290?casa_token=Rr8iWs71uhYAAAAA:D4PWThLU5hKi7khAv3yk23pR76hR81P5dTDSUjLJrF5SPL2r76hZE3YkHOGPzapU64pAzzHuAgU#!)
- #PAPER [Single-blind validation of space-based point-source methane emissions detection and quantification (Sherwin 2022)](https://eartharxiv.org/repository/view/3465/)
- #PAPER [METER-ML: A Multi-sensor Earth Observation Benchmark for Automated Methane Source Mapping (Zhu 2022)](https://stanfordmlgroup.github.io/projects/meter-ml/)
	- multi-sensor Earth observation dataset containing georeferenced images in the U.S. labeled for the presence or absence of six methane source facilities




