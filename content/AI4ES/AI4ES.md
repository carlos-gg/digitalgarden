---
title: "AI4ES"
---

> Applications of [[AI/Machine Learning]] and [[AI/AI]] to Earth Sciences

## Resources
- [Earth system science](https://en.wikipedia.org/wiki/Earth_system_science)
- [Accelerating progress in Climate Science (Schneider 2021, Physics today)](https://digital.physicstoday.org/physicstoday/june_2021/MobilePagedReplica.action?utm_source=newsletter&utm_medium=email&utm_campaign=TXPHYS210602002&utm_content=gtxcel&pm=2&folio=44#pg47)
- https://www.scientificamerican.com/article/how-machine-learning-could-help-to-improve-climate-forecasts/
- https://e360.yale.edu/features/can-artificial-intelligence-help-build-better-smarter-climate-models
- [Artificial Intelligence—A Game Changer for Climate Change and the Environment ](https://blogs.ei.columbia.edu/2018/06/05/artificial-intelligence-climate-environment/)
- [Ten Ways to Apply Machine Learning in Earth and Space Sciences](https://eos.org/opinions/ten-ways-to-apply-machine-learning-in-earth-and-space-sciences)
- [Supercomputers, Climate Models and 40 Years of the World Climate Research Programme](https://insideclimatenews.org/news/06122019/climate-models-supercomputer-world-research-program-agu-100-anniversary-cheyenne-wyoming)
- [Thoughtfully Using Artificial Intelligence in Earth Science](https://eos.org/opinions/thoughtfully-using-artificial-intelligence-in-earth-science)
- [Advancing AI for Earth Science: A Data Systems Perspective](https://eos.org/science-updates/advancing-ai-for-earth-science-a-data-systems-perspective)
	- high-priority challenges include:
		- a lack of publicly available benchmark training data sets across all science disciplines
		- a lack of interoperability among data sources, types, and formats (e.g., standard data formats for computer vision algorithms may be different from the standard formats for commonly used Earth science models)
		- limited availability of baseline pretrained models that can be customized for various types or modes of Earth observations
		- label or target values that are not usually structured, such as oceanic measurements from drifting buoys that cannot be adapted easily to the grid systems commonly used in ML algorithms
- [Weathering Environmental Change Through Advances in AI](https://eos.org/opinions/weathering-environmental-change-through-advances-in-ai)
- [Tackling 21st Century Geoscience Problems with Machine Learning](https://eos.org/editors-vox/tackling-21st-century-geoscience-problems-with-machine-learning)
- [Advancing Application of Machine Learning Tools for NASA’s Earth Observation Data (NASA)](https://cdn.earthdata.nasa.gov/conduit/upload/14287/NASA_ML_Workshop_Report.pdf) ^7b7470
- [Training the Next Generation of Physical Data Scientists](https://eos.org/opinions/training-the-next-generation-of-physical-data-scientists)

## Talks
- #TALK [Deep Learning for Climate (Gallinari)](https://ai4climate.lip6.fr/wp-content/uploads/2018/10/2018-05-25-Deep-Learning-Climate-Gallinari-2.pdf)

## Books
- #BOOK [Introduction to Climate Science (Schmittner 2017)](https://open.umn.edu/opentextbooks/textbooks/introduction-to-climate-science-1st-edition-schmittner)
- #BOOK [Introduction to Oceanography (Webb 2019)](https://open.umn.edu/opentextbooks/textbooks/introduction-to-oceanography)
- #BOOK [Introduction to Environmental Science - 2nd Edition (2018)](https://open.umn.edu/opentextbooks/textbooks/introduction-to-environmental-science-2nd-edition)
- #BOOK [Introduction to Physical Oceanography (Stewart 2008)](https://open.umn.edu/opentextbooks/textbooks/introduction-to-physical-oceanography)

## Courses
- #COURSE [An Introduction to Earth and Environmental Data Science (Ryan Abernathey, Columbia UIniversity, 2021)](https://earth-env-data-science.github.io/intro.html)
- #COURSE [Research computing in ES (Ryan Abernathey, Columbia UIniversity)](https://rabernat.github.io/research_computing_2018/)
- #COURSE [Introduction to Environmental Data Science (Jerry Davis, SFSU Institute for Geographic Information Science_, 2022)](https://bookdown.org/igisc/EnvDataSci/)

## References
> See:
> - [[AI4ES/EO]]
> - [[AI4ES/Geospatial science]]

- #PAPER [Earth System Modeling 2.0: A Blueprint for Models That Learn From Observations and Targeted High‐Resolution Simulations (Schneider 2017)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2017GL076101)
	- http://climate-dynamics.org/earth-system-modeling-2-0/
	- ESM with subgrid-scale (SGS) process models that learn automatically from two sources of information
		- Global observations. ESMs can learn directly from space-based global data, augmented and validated with more detailed local observations where available
		- Local high-resolution simulations. Some SGS processes in ESMs are in principle computable, only the globally achievable resolution precludes their explicit computation
	- The automated learning from observations and high-resolution simulations will use statistics accumulated in time (e.g., over seasons) to:
		- Minimize model biases, especially biases that are known to correlate with the climate response of models. This amounts to minimizing mismatches between time averages of ESM-simulated quantities and data
		- Minimize model-data mismatches in higher-order Earth system statistics
- #PAPER [Machine learning for data-driven discovery in solid Earth geoscience (Bergen 2019)](https://science.sciencemag.org/content/363/6433/eaau0323)
- #PAPER [Machine learning and artificial intelligence to aid climate change research and preparedness (Huntingford et al., 2019)](https://iopscience.iop.org/article/10.1088/1748-9326/ab4e55)
	- Nine basic dimensions of climate modelling (there include geographical location, the many configurations of ESMs, and alternative future trajectories in emissions policy) : Longitude direction, altitude direction, Vertical direction, Time, Different climate models, Climate model ensembles, Different initial state, Perturbed physics runs, Different future emissions
	- Examples of existing [[AI]] applications to climate: Earth System modelling, Teleconnections, Weather forecasting, Future climate scenarios, Climate impacts, Climate datasets, Climate extremes
- #PAPER [Leveraging Modern Artificial Intelligence for Remote Sensing and NWP: Benefits and Challenges (Boukabara 2019)](https://journals.ametsoc.org/bams/article/100/12/ES473/344464/Leveraging-Modern-Artificial-Intelligence-for)
- #PAPER [Deep learning and process understanding for data-driven Earth system science (Reichstein, 2019)](https://doodle.com/poll/r5fwu4rne37hzkgh?utm_source=poll&utm_medium=link)
	- http://www.ccpo.odu.edu/~klinck/Reprints/PDF/reichsteinNature2019.pdf
	- ML approaches are increasingly used to extract patterns and insights from the ever-increasing stream of geospatial data, but current approaches may not be optimal when system behaviour is dominated by spatial or temporal context
	- Earth system data are exemplary of all four of the ‘four Vs’ of ‘big data’: volume, velocity, variety and veracity
	- One key challenge is to extract interpretable information and knowledge from this big data, possibly almost in real time and integrating between disciplines
	- Two major tasks in the coming years: (1) extracting knowledge from the data deluge, and (2) deriving models that learn much more from data than traditional data assimilation approaches can, while still respecting our evolving understanding of nature’s laws
	- #TALK [Machine-learning-model-data-integration for a better understanding of the Earth System (Markus Reichstein)](https://events.ecmwf.int/event/227/ ) ^ea6338
- #PAPER [Machine Learning for Clouds and Climate (Beucler 2020)](https://www.semanticscholar.org/paper/Machine-Learning-for-Clouds-and-Climate-Beucler-Ebert%E2%80%90Uphoff/ea0ccde42b1f4517e87ee2e3f77fb6c06671666b)
- #PAPER [What is next for National Meteorological Services? (Arribas 2020)](https://arxiv.org/abs/2005.01425)
	- Head of informatics lab at Met  office, Prof. U. Exeter, Turing fellow
	- #TALK [[AI]], a change in science/technology ... or culture? 
		- https://vimeo.com/438176732
		- https://www.ecmwf.int/sites/default/files/medialibrary/2020-07/14_July_Arribas.pdf
- #PAPER [A digital twin of Earth for the green transition (Bauer 2021)](https://www.nature.com/articles/s41558-021-00986-y)
	- A digital twin of Earth is an information system that exposes users to a digital replication of the state and temporal evolution of the Earth system constrained by available observations and the laws of physics
	- Digital twins must focus exactly on how best to realize this convergence of the modelling and observation worlds
	- A methodological framework for the twin’s architecture already exists in the form of data assimilation, which numerical weather prediction has developed with success over decades
- #PAPER [Machine learning for weather and climate are worlds apart (Watson-Parris 2021)](https://royalsocietypublishing.org/doi/10.1098/rsta.2020.0098)
- #PAPER [Evolution of machine learning in environmental science—A perspective (Hsieh 2022)](https://www.cambridge.org/core/journals/environmental-data-science/article/evolution-of-machine-learning-in-environmental-sciencea-perspective/C21F19C66FA387BC25F43C3C6B95E866)
- #PAPER [Machine Learning in Weather Prediction and Climate Analyses—Applications and Perspectives (Bochenek 2022)](https://www.mdpi.com/2073-4433/13/2/180/htm)

### AI for pattern recognition and spatio-temporal modelling
- See [[AI/Computer Vision/Video segmentation and prediction]]
- Extreme events identification. See [[AI4ES/Extremes events]]
- See [[Weather forecasting, nowcasting#^e83f4e]]

### Climate models
See [[AI4ES/ESMs, GCMs]], [[AI4ES/Ensembles, multi-models]] and [[AI4ES/Weather forecasting, nowcasting]], [[AI/Computer Vision/Image-to-image translation]], [[AI/Computer Vision/Video segmentation and prediction]] (next frame prediction) using the temporal dimension

### Filling observational gaps
See [[AI4ES/Filling observational gaps]]

### S2S2D
See [[AI4ES/S2S]], [[AI4ES/S2D]]

### Parameterizations
See [[AI4ES/Parameterizations]]

### Atmospheric composition and air quality
See [[AI4ES/AC, AQ]]

### Statistical downscaling
See [[AI4ES/Statistical downscaling]]

### Bias correction and adjustment
See [[AI4ES/Bias correction, adjustment]]

### HPC and distributed DL/ML
See [[AI/DS and DataEng/Distributed DL]] and [[AI4ES/HPC-AI convergence]]

### ML interpretability and causal modelling in ES
See [[AI4ES/ML interpretability in ES]] and [[AI4ES/Causal modeling in ES]]

### Digital twins
See [[AI4ES/Emulators]]
- [NVIDIA Construirá la Supercomputadora Earth-2 para Ver Nuestro Futuro](https://la.blogs.nvidia.com/2021/11/16/supercomputadora-earth-2/)
- [Climate Science Sessions at GTC Highlight How Digital Twins Powered by HPC and AI Can Help Earth](https://blogs.nvidia.com/blog/2022/03/08/climate-science-sessions-gtc/)
- #PAPER [How to tell the difference between a model and a digital twin (Wright 2020)](https://amses-journal.springeropen.com/articles/10.1186/s40323-020-00147-4)

### Other applications
#### Agriculture
- #PAPER [Deep learning in agriculture: A survey (Kamilaris 2018)](http://arxiv.org/abs/1807.11809)
- #PAPER [Machine Learning in Agriculture: A Review (Liakos 2018)](https://www.mdpi.com/1424-8220/18/8/2674/htm)
- #PAPER [Crop yield prediction using machine learning: A systematic literature review (van Klompenburg 2020)](https://www.sciencedirect.com/science/article/pii/S0168169920302301?dgcid=rss_sd_all)

#### Smart buildings
- #PAPER [Leveraging Machine Learning and Big Data for Smart Buildings: A Comprehensive Survey (Qolomany 2019)](https://www.researchgate.net/publication/332170623_Leveraging_Machine_Learning_and_Big_Data_for_Smart_Buildings_A_Comprehensive_Survey )
- #PAPER [Physics-constrained deep learning of multi-zone building thermal dynamics (Drgona 2021)](https://www.sciencedirect.com/science/article/pii/S0378778821002760#f0010)

#### Compression of Climate model outputs
- #PAPER [Evaluating lossy data compression on climate simulation data within a large ensemble (Baker 2016)](https://gmd.copernicus.org/articles/9/4381/2016/)
- #PAPER [A statistical analysis of lossily compressed climate model data (Poppick 2020)](https://www.sciencedirect.com/science/article/pii/S009830042030580X)
- #PAPER [Compressing atmospheric data into its real information content (Kloewer 2022)](https://www.researchsquare.com/article/rs-590601/v1)
	- #CODE https://github.com/esowc/Elefridge.jl

#### Energy optimization and renewable energy
- #PAPER [Surrogate modelling for sustainable building design – A review (Westermann 2019)](https://www.sciencedirect.com/science/article/abs/pii/S0378778819302877)
- #PAPER [Building energy optimization using surrogate model and active sampling (Bamdad 2020)](https://www.tandfonline.com/doi/full/10.1080/19401493.2020.1821094)
- #PAPER [Using a deep temporal convolutional network as a building energy surrogate model that spans multiple climate zones (Westermann 2020)](https://www.sciencedirect.com/science/article/abs/pii/S0306261920310758)
- #PAPER [Machine Learning for Sustainable Energy Systems (Donti 2021)](https://www.annualreviews.org/doi/abs/10.1146/annurev-environ-020220-061831)

### Computational Fluid Dynamics (CFD)
 #PAPER [Accelerating urban scale simulations leveraging local spatial 3D structure (Iserte 2022)](https://www.sciencedirect.com/science/article/pii/S1877750322001326)


## Infrastructure and data
See [[AI4ES/AI4ES data]]
- [Microsfot Planetary Computer](https://planetarycomputer.microsoft.com/)
- [European Weather Cloud](https://www.europeanweather.cloud/)
	- https://www.ecmwf.int/en/newsletter/165/computing/progress-towards-european-weather-cloud
- [Climate Engine](http://climateengine.org/)
- [The OpenWIS Association AISBL](http://openwis.github.io/openwis-documentation/)
- [Euro Data Cube](https://www.eurodatacube.com/)
	- https://hub.eox.at/marketplace/notebooks
- [Ocean OPS](https://www.ocean-ops.org/board)
	- Integrated information, maps and tools to help coordinate and monitor global ocean observation efforts
- [EUMETSAT data portal](https://www.eumetsat.int/who-we-work/access-copernicus-data)
	- [EUMETView](https://view.eumetsat.int/productviewer?v=default)
	- [Product navigator](https://navigator.eumetsat.int/start)
- AI4ES/Pangeo Forge. See [[AI4ES/Pangeo]]

## Code
See [[AI4ES/Pangeo]]
- #CODE [Lexcube - Leipzig explorer of Earth data cubes](https://www.lexcube.org/)
- #CODE [xcast](https://github.com/kjhall01/xcast)
	- A High-Performance Data Science Toolkit for the Earth Sciences
- #CODE [climate_indices](https://github.com/monocongo/climate_indices)
	- Climate indices for drought monitoring, community reference implementations in Python
- #CODE [CliMetLab - Python package to easy access to weather and climate data](https://github.com/ecmwf/climetlab)
	- https://climetlab.readthedocs.io/en/latest/index.html
- #CODE [intake - lightweight package for finding, investigating, loading and disseminating data](https://github.com/intake/intake)
	- https://medium.com/pangeo/cesm-lens-on-aws-4e2a996397a1
	- [example](https://aws-uswest2-binder.pangeo.io/v2/gh/NCAR/cesm-lens-aws/master?urlpath=lab)
	- https://www.anaconda.com/blog/intake-discovering-and-exploring-data-in-a-graphical-interface
- #CODE [intake-esm - An intake plugin for parsing an Earth System Model (ESM) catalog and loading assets into xarray datasets](https://github.com/intake/intake-esm)
	- https://intake-esm-test.readthedocs.io
- #CODE [Aospy - Python package for automated analysis and management of gridded climate data](https://github.com/spencerahill/aospy)
- #CODE [EarthPy](https://github.com/earthlab/earthpy)
	- A package built to support working with spatial data using open source python
	- https://earthpy.readthedocs.io/en/latest/
- #CODE [Psyplot - Python package for interactive data visualization](https://github.com/psyplot/psyplot)
	- https://psyplot.readthedocs.io/en/latest/
	- https://psyplot.readthedocs.io/projects/psyplot-gui/en/latest/index.html#psyplot-gui
	- https://psyplot.readthedocs.io/projects/psy-view/en/latest/index.html#psy-view
- #CODE [PyRain](https://github.com/FrontierDevelopmentLab/PyRain)
	- [[AI4ES/AI4ES data#^rainbench]]
- #CODE [Verde](https://github.com/fatiando/verde)
	- Processing and interpolating spatial data with a twist of machine learning
	- https://github.com/fatiando/verde
	- https://www.fatiando.org/verde/latest/index.html
- #CODE [Radiant MLHub API](https://github.com/radiantearth/radiant-mlhub)
	- Open Library for Earth Observations Machine Learning
	- https://www.radiant.earth/mlhub/
	- https://github.com/radiantearth/mlhub-tutorials
	- [Radiant MLHub](https://www.mlhub.earth/#datasets)
- #CODE [GIBS Downloader](https://github.com/spaceml-org/GIBS-Downloader)
	- command-line tool which facilitates the downloading of NASA satellite imagery and offers different functionalities in order to prepare the images for training in a machine learning pipeline
	- #CODE https://github.com/spaceml-org/Self-Supervised-Learner


## Events
- See [[AI4ES/EO#Events]] and [[AI4ES/Geospatial science#Events]]
- Conferences, events, workshops and courses related to [[AI/AI]], [[AI4ES/EO]], [[AI4ES/Geospatial science]] and [[AI/Machine Learning]] applied to Earth Sciences.
- [AI for Good. Discovery - AI and Climate Science](https://aiforgood.itu.int/eventcat/discovery-ai-and-climate-science/)
- https://spcl.inf.ethz.ch/Bcast/

### 2022
- [ECMWF-ESA Workshop on Machine Learning for Earth Observation and Prediction](https://events.ecmwf.int/event/304/)
- [Weather and Climate Extremes and their Predictability](http://www.cafes2se-itn.eu/weather-and-climate-extremes-and-their-predictability-cafe-final-conference)
- [SIAM Conference on Imaging Science (IS22)](https://www.siam.org/conferences/cm/conference/is22). March 22 - 25, 2022
- [21st Conference on Artificial Intelligence for Environmental Science](https://annual.ametsoc.org/index.cfm/2022/program-events/conferences-and-symposia/21st-conference-on-artificial-intelligence-for-environmental-science/)
- https://www.iarai.ac.at/workshops/workshop-on-complex-data-challenges-in-earth-observation-2022/
- [Climate informatics 2022](https://ncics.org/news/events/ci2022/agenda/)
	- [handbook](https://docs.google.com/document/d/1p1CvnK1TVaLAXOCN0vpnsQxvWIGVmjpt-WXD4g0CH2E/edit?usp=sharing)
	- [Q&A](https://app.sli.do/event/uJr35rXEM9ChavrRSAhnig/live/questions)
	- https://app.wonder.me/?spaceId=7b51f530-f040-40ce-a108-f06b53c18752

### 2021
- [Trustworthy Artificial Intelligence for Environmental Science (TAI4ES) Summer School](https://www2.cisl.ucar.edu/tai4es)
	- [Recording and slides](https://docs.google.com/document/d/1qKGbbYKswzftWKmQpfMU08LTUmBjYXGO8XY9ueB782k/edit?usp=sharing)
- [ESA-ECMWF WORKSHOP. Machine Learning for Earth System Observation and Prediction](https://nikal.eventsair.com/esa-ecmwf-workshop-2021/)
- [Machine learning for numerical weather predictions and climate services – A workshop for Member and Co-operating States](https://ecmwfevents.com/i/b73a4e9a-79ab-4e27-879c-d885e895cdeb/login)
	- https://events.ecmwf.int/event/239/timetable/
- [ICML 2021 - Workshop Tackling Climate Change with Machine Learning](https://www.climatechange.ai/events/icml2021#about-the-workshop)
- [WCRP Workshop on Extremes in Climate Prediction Ensembles (ExCPEns) (2021 TBD)](https://apcc21.org/act/work.do?lang=en&bbsId=BBSMSTR_000000000024)
- [2020 -> 2021. ASP Colloquium "The Science Of Subseasonal To Seasonal (S2S) Predictions"](https://staff.ucar.edu/for-staff/daily/announcement/2020-asp-colloquium-science-subseasonal-seasonal-s2s-predictions-now)
- [EGU 2021](https://www.egu21.eu/)
- [19th Workshop on high performance computing in meteorology](https://events.ecmwf.int/event/169/)
- [ECMWF - Virtual workshop: Weather and climate in the cloud](https://events.ecmwf.int/event/211/)
- [Workshop on "Machine Learning Advances Environmental Science (MAES)" - organised in conjunction with The 25th International Conference on Pattern Recognition (Milan, Italy, January 10-15, 2021)](https://sites.google.com/view/maes-icpr2020/)
- [AMS101 (10-14 january 2021)](https://annual.ametsoc.org/index.cfm/2021/)
	- https://annual.ametsoc.org/index.cfm/2021/program-events/conferences-and-symposia/34th-conference-on-climate-variability-and-change/
	- https://annual.ametsoc.org/index.cfm/2021/program-events/conferences-and-symposia/20th-conference-on-artificial-intelligence-for-environmental-science/
	- https://annual.ametsoc.org/index.cfm/2021/program-events/conferences-and-symposia/seventh-symposium-on-high-performance-computing-for-weather-water-and-climate/
- [PASC21](https://pasc21.pasc-conference.org/)
- [The ENES Climate Analytics Service (ECAS) online training](https://is.enes.org/events/trainings-and-education/joint-is-enes3-eosc-hub-online-training-event-on-data-analytics-with-enes-climate-analytics-service-ecas)
	- https://global.gotomeeting.com/join/415422533
	- https://github.com/IS-ENES-Data/Climate-data-analysis-service
	- https://github.com/ECAS-Lab/ecas-training
	- https://portal.enes.org/data/data-metadata-service/enes-climate-analytics-service-ecas
	- [Slides, resources](https://drive.google.com/drive/folders/1Af5GlUV27kZpoIpC6BHMXCHlZmq59232)
- IS-ENES3/ESiWACE2 New Opportunities for AI/ML in weather/climate modelling

### 2020
- [Environmental Intelligence Conference](https://www.bigmarker.com/JCEEI/JCEEI-Environmental-Intelligence-Conference-Thursday-17th-December)
- [ECMWF-ESA Workshop on Machine Learning for Earth System Observation and Prediction (5-8 October 2020)](https://www.ecmwf.int/en/learning/workshops/ecmwf-esa-workshop-machine-learning-earth-system-observation-and-prediction)
- [Machine Learning for Earth Observation, In Conjunction with the ECML/PKDD 2020 (September)](https://sites.google.com/view/maclean2020/)
- NCAR Artificial Intelligence for Earth System Science (AI4ESS) Summer School
	- https://www2.cisl.ucar.edu/events/summer-school/ai4ess/2020/artificial-intelligence-earth-system-science-ai4ess-summer-school
	- [Slides](https://www2.cisl.ucar.edu/events/summer-school/ai4ess/2020/presentation-slides)
	- #TALK https://www2.cisl.ucar.edu/events/summer-school/ai4ess/2020/presentation-recordings
	- #CODE https://github.com/NCAR/ai4ess-hackathon-2020
- [10th CCI colocation meeting](https://nikal.eventsair.com/10th-cci-colocation-meeting/esa)
- [Workshop "Data Science in Climate and Climate Impact Research" (August 20 afternoon and 21, 2020)](https://wcr.ethz.ch/news-and-events/events/workshop--data-science-in-climate-and-climate-impact-research-.html)
- [Climate informatics (September 23-25, 2020)](https://ci2020.web.ox.ac.uk/call-papers)
- NeurIPS 2020.
	- [AI for Earth Sciences](https://ai4earthscience.github.io/neurips-2020-workshop/)
- ICLR 2020. 
	- [AI for Earth Sciences](https://ai4earthscience.github.io/iclr-2020-workshop/)
	- Tackling CC with ML: 
		- https://www.climatechange.ai/events/iclr2020.html
		- https://slideslive.com/iclr-2020/workshop-tackling-climate-change-with-ml
- [6th ENES HPC workshop](https://www.esiwace.eu/events/6th-hpc-workshop/6th-hpc-workshop)
- [Radiant Earth NASA ML Workshop](https://www.radiant.earth/events/nasa-ml-2020/ ^nasamlws)
	- https://www.youtube.com/playlist?list=PL3QzFgBMGnbQRa8uHP0_C_P2Fl5GIBxmn
- [1st Workshop on Knowledge Guided Machine Learning (KGML)](https://sites.google.com/umn.edu/kgml/workshop)

### 2019
- [Machine Learning for Weather and Climate Modelling (Oxford UK, 2019)](http://users.ox.ac.uk/~phys0895/mlwc2019/index.html)
- [The 1st Artificial Intelligence for Copernicus Workshop (Reading UK, 2019)](https://atmosphere.copernicus.eu/1st-artificial-intelligence-copernicus-workshop)
- [Big Data Summit 2019: AI and HPC Convergence for Science](https://www.nersc.gov/research-and-development/data-analytics/big-data-center/big-data-summit-2019/)



