---
title: "EO"
---

## Resources
- [Towards a European [[AI]] for Earth Observation Research & Innovation Agenda](http://blogs.esa.int/philab/files/2018/07/Towards-a-European-AI-for-Earth-Observation-Research-Innovation-Agenda-.pdf)
- [Mapping roads through deep learning and weakly supervised training](https://ai.facebook.com/blog/mapping-roads-through-deep-learning-and-weakly-supervised-training/)
- [Example of SuperRes with Sentinel 2 data](https://mdl4eo.irstea.fr/2019/03/29/enhancement-of-sentinel-2-images-at-1-5m/  )
- [Quantifying the surface area of road networks in cities](https://roadsfromabove.netlify.com/)
	- Nice visualization
- [CNN-Sentinel](https://github.com/jensleitloff/CNN-Sentinel)
	- Analyzing Sentinel-2 satellite data in Python with Keras (repository of our talks at Minds Mastering Machines 2019 and PyCon 2018)
- https://interestingengineering.com/mapping-every-solar-panel-in-the-world-with-machine-learning
- [Image Classification with Hugging Face Transformers and Keras (EuroSAT dataset)](https://www.philschmid.de/image-classification-huggingface-transformers-keras)

## Courses
- #COURSE [Artificial Intelligence (AI) for Earth Monitoring](https://www.futurelearn.com/courses/artificial-intelligence-for-earth-monitoring)
- #COURSE [ESA ML lectures 2018](https://github.com/jmartinezheras/2018-MachineLearning-Lectures-ESA)

## Code
- #CODE [TorchGeo (Microsoft)](https://github.com/microsoft/torchgeo)
	- https://torchgeo.readthedocs.io/
- #CODE [Raster vision](https://github.com/azavea/raster-vision)
	- https://docs.rastervision.io/en/0.13/
- #CODE [Google Earth Engine](https://developers.google.com/earth-engine/)
	- https://developers.google.com/earth-engine/datasets/catalog
	- https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR
	- https://developers.google.com/earth-engine/datasets/catalog/ECMWF_ERA5_DAILY
- #CODE [eo-learn: eo-learn makes extraction of valuable information from satellite imagery easy](https://github.com/sentinel-hub/eo-learn)
- #CODE [OpenEO - A Common, Open Source Interface between Earth Observation Data Infrastructures and Front-End Applications](https://github.com/open-eo)
- #CODE [Satpy - package is a python library for reading and manipulating meteorological remote sensing data and writing it to various image and data file formats](https://github.com/pytroll/satpy)
- #CODE [rasterio - access to geospatial raster data](https://github.com/mapbox/rasterio)
- #CODE [EODAG - Earth Observation Data Access Gateway](https://github.com/CS-SI/eodag)
	- https://eodag.readthedocs.io/en/latest/
	- https://www.youtube.com/watch?v=R18yTXKhF-I&list=PLvT7fd9OiI9XORxAfLw_f9CsDkvM9lfKs&index=23

## References
Review papers:
- #PAPER [Survey of Deep Learning Approaches for Remote Sensing Observation Enhancement (Tsagkatakis 2019)](https://www.mdpi.com/1424-8220/19/18/3929)

- #PAPER [Machine Learning Applications for Earth Observation (Lary 2018)](https://www.researchgate.net/publication/322659251_Machine_Learning_Applications_for_Earth_Observation)
- #PAPER [Learning Spectral-Spatial-Temporal Features via a Recurrent Convolutional Neural Network for Change Detection in Multispectral Imagery (Mou 2018)](https://arxiv.org/abs/1803.02642 )
- #PAPER [Multi-Stream [[CNNs]] for SAR Automatic Target Recognition (Zhao 2018)](https://www.mdpi.com/2072-4292/10/9/1473)
- #PAPER [Multi-Temporal Land Cover Classification with Sequential Recurrent Encoders (Rubwurm 2018)](http://arxiv.org/abs/1802.02080)
- #PAPER [Dialectical [[GANs]] for SAR Image Translation: From Sentinel-1 to TerraSAR-X  (Ao 2018)](https://arxiv.org/abs/1807.07778)
- #PAPER [Machine Learning Using Hyperspectral Data Inaccurately Predicts Plant Traits Under Spatial Dependency (Rocha 2018)](https://www.mdpi.com/2072-4292/10/8/1263)
- #PAPER [Satellite Imagery Multiscale Rapid Detection with Windowed Networks (Van Etten 2018)](https://arxiv.org/abs/1809.09978)
	- #CODE https://github.com/avanetten/simrdwn
	-  The SIMRDWN pipeline includes a modified version of YOLO (known as YOLT), along with the models of the tensorflow object detection API: SSD, Faster R-CNN, and R-FCN
- #PAPER [[[AI]] [[AI/DS and DataEng/Data Science]] Methodology for Earth Observation (Dumitru 2019)](https://www.intechopen.com/books/advanced-analytics-and-artificial-intelligence-applications/artificial-intelligence-data-science-methodology-for-earth-observation)
- #PAPER [Next Generation Mapping: Combining [[AI/Deep learning/DL]], Cloud Computing, and Big Remote Sensing Data (Parente 2019)](https://www.mdpi.com/2072-4292/11/23/2881)
- #PAPER [Temporal [[CNNs]] for the Classification of Satellite Image Time Series (Pelletier 2019)](https://arxiv.org/abs/1811.10166)
- #PAPER [Combining Sentinel-1 and Sentinel-2 Satellite Image Time Series for land cover mapping via a multi-source deep learning architecture (Ienco 2019)](https://www.sciencedirect.com/science/article/abs/pii/S0924271619302278?via%3Dihub)
- #PAPER [The Challenge of Machine Learning in Space Weather: Nowcasting and Forecasting (Camporeale 2019)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018SW002061)
	- New trends in ML: Physics‐informed NNs, Automatic machine learning, Adversarial training.
	- Future challenges in ML for space weather: The information problem, The gray‐box problem, The surrogate problem (What components in the Space Weather chain can be replaced by an approximated black‐box surrogate model?), The uncertainty problem (Assessing the uncertainty associated to Weather predictions), The too often too quiet problem (data sets are typically imbalanced. Use synthetic data? Use simulated data), The knowledge discovery problem (How do we distill some knowledge from a machine learning model and improve our understanding of a given system? How do we open the black‐box and reverse‐engineer a machine learning algorithm?)
- #PAPER [Machine Learning for Precipitation Nowcasting from Radar Images (Agrawal 2019)](https://arxiv.org/abs/1912.12132)
	- https://ai.googleblog.com/2020/01/using-machine-learning-to-nowcast.html
- #PAPER [Feature Extraction and Classification Based on Spatial-Spectral ConvLSTM Neural Network for Hyperspectral Images (Hu 2019)](https://arxiv.org/abs/1905.03577)
	- ConvLSTM 3-D
- #PAPER [[[AI/Deep learning/DL]] meets SAR (Xiang Zhu 2020)](https://arxiv.org/abs/2006.10027v1)
- #PAPER [Sentinel-2 Sharpening via Parallel Residual Network (Wu 2020)](https://www.mdpi.com/2072-4292/12/2/279/htm)
- #PAPER [Spectral Variability in Hyperspectral Data Unmixing: A Comprehensive Review (Borsoi 2020)](http://arxiv.org/abs/2001.07307)
- #PAPER [Nonlinear PCA for Spatio-Temporal Analysis of Earth Observation Data (Bueso 2020)](https://arxiv.org/abs/2002.04539)
	- #CODE https://github.com/DiegoBueso/ROCK-PCA
	- Dimensionality  reduction  methods  can  work  with  spatio-temporal datasets and decompose the information efficiently. Principal Component Analysis (PCA), also known as Empirical Orthogonal Functions (EOF) in geophysics, has been traditionally used to analyze climatic data
	- When nonlinear feature relations are present, PCA/EOF fails
	- Propose a nonlinear PCA method to deal with spatio-temporal Earth System data
	- The proposed method, called Rotated Complex Kernel PCA (ROCK-PCA for short), works in reproducing kernel Hilbert spaces to account for nonlinear processes, operates in the complex kernel domain to account for both space and time features, and adds an extra rotation for improved flexibility
	- Results of the decomposition of three essential climate variables are shown: satellite-based global Gross Primary Productivity (GPP) and Soil Moisture (SM), and reanalysis Sea Surface Temperature (SST) data
	- The ROCK-PCA method allows identifying their annual and seasonal oscillations, as well as their non-seasonal trends and spatial variability patterns.
- #PAPER [Accounting for Training Data Error in Machine Learning Applied to Earth Observations (Elmes 2020)](https://www.mdpi.com/2072-4292/12/6/1034/htm)
- #PAPER [Uncertainty Quantification in Machine Learning Modeling for Multi-Step Time Series Forecasting:Example of Recurrent Neural Networks in Discharge Simulations (Song 2020)](https://www.mdpi.com/2073-4441/12/3/912/htm)
- #PAPER [Model and data uncertainty for satellite time series forecasting with deep recurrent models (Rubwurm 2020)](https://elib.dlr.de/139306/1/igarss2020_tex.pdf)
- #PAPER [Living in the Physics and Machine Learning Interplay for Earth Observation (Camps-Valls 2020)](https://arxiv.org/abs/2010.09031)
- #PAPER [NightVision: Generating Nighttime Satellite Imagery from Infra-Red Observations (Harder 2020)](https://arxiv.org/abs/2011.07017)
- #PAPER [DEEPCUBE: Explainable AI pipelines for big Copernicus data (Papoutsis 2021)](http://cgi.di.uoa.gr/~koubarak/publications/2021/BIDS21_paper54.pdf) ^deepcube
- #PAPER [Towards global flood mapping onboard low cost satellites with machine learning (Mateo-Garcia 2021)](https://www.nature.com/articles/s41598-021-86650-z)
- #PAPER [A generalizable and accessible approach to machine learning with global satellite imagery (Rolf 2021)](https://www.nature.com/articles/s41467-021-24638-z)
	- #CODE https://github.com/Global-Policy-Lab/mosaiks-paper
	- https://cega.berkeley.edu/research/mosaiks-a-generalizable-and-accessible-approach-to-machine-learning-with-global-satellite-imagery/
	- #TALK https://cega.berkeley.edu/resource/video-afternoon-keynotes-catherine-wolfram-sol-hsiang-infra4dev-2020/
	- ML system to tap the problem-solving potential of satellite imaging, using low-cost, easy-to-use technology that could bring access and analytical power to researchers and governments worldwide


### Object detection/recognition
- #PAPER [Object Detection in Optical Remote Sensing Images: A Survey and A New Benchmark (Li 2019)](https://arxiv.org/abs/1909.00133) ^dior
- #PAPER [Object Detection in Remote Sensing Images Based on Improved Bounding Box Regression and Multi-Level Features Fusion (Qian 2020)](https://www.mdpi.com/2072-4292/12/1/143/htm)
- #PAPER [An Enriched Automated PV Registry: Combining Image Recognition and 3D Building Data (Rausch 2020)](https://www.climatechange.ai/papers/neurips2020/46/paper.pdf)
	- #CODE https://github.com/kdmayer/PV4GER
	- computer vision-based pipeline leveraging aerial imagery with a spatial resolution of 10 cm/pixel and 3D building data to automatically create address-level PV registries for all counties within Germany's most populous state North Rhine-Westphalia
- #PAPER [FAIR1M: A Benchmark Dataset for Fine-grained Object Recognition in High-Resolution Remote Sensing Imagery (Sun 2021)](https://arxiv.org/abs/2103.05569) ^fair1m


### Semantic segmentation
- #PAPER [Multi3Net: Segmenting Flooded Buildings via Fusion of Multiresolution, Multisensor, and Multitemporal Satellite Imagery (Rudner 2018)](https://arxiv.org/abs/1812.01756)
- #PAPER [Wide-Area Land Cover Mapping with Sentinel-1 Imagery using [[AI/Deep learning/DL]] Semantic Segmentation Models (Scepanovic 2020)](https://arxiv.org/abs/1912.05067v2)
- #PAPER [Dense Dilated Convolutions Merging Network for Land Cover Classification (Liu 2020)](https://arxiv.org/abs/2003.04027v1)
- #PAPER [Continental-Scale Building Detection from High Resolution Satellite Imagery (Sirko 2021)](https://arxiv.org/abs/2107.12283)
	- https://ai.googleblog.com/2021/07/mapping-africas-buildings-with.html
- #PAPER [Semantic segmentation of PolSAR image data using advanced deep learning model (Garg 2021)](https://www.nature.com/articles/s41598-021-94422-y)
- #PAPER [A Dual Network for Super-Resolution and Semantic Segmentation of Sentinel-2 Imagery (Abadal 2021)](https://www.mdpi.com/2072-4292/13/22/4547/htm)
	- https://imatge.upc.edu/web/publications
- #PAPER [Evaluation of Semantic Segmentation Methods for Land Use with Spectral Imaging Using Sentinel-2 and PNOA Imagery (Pedrayes 2021)](https://www.mdpi.com/2072-4292/13/12/2292/htm)
- #PAPER [Semantic segmentation of slums in satellite images using transfer learning on fully convolutional neural networks (Wurm 2019)](https://www.sciencedirect.com/science/article/pii/S0924271619300383)

### Super-resolution
See:
[[Super-resolution]]
[[AI4ES/Statistical downscaling]]
Review papers:
- #PAPER [Deep Learning for Single Image Super-Resolution:A Brief Review (Yang 2019)](https://arxiv.org/abs/1808.03344)

- #PAPER [PanNet: A deep network architecture for pan-sharpening (Yang 2017)](http://openaccess.thecvf.com/content_iccv_2017/html/Yang_PanNet_A_Deep_ICCV_2017_paper.html)
	- #CODE https://github.com/oyam/PanNet-Landsat
- #PAPER [Target-adaptive CNN-based pansharpening (Scarpa 2018)](https://arxiv.org/abs/1709.06054)
- #PAPER [Super-resolution of Sentinel-2 images: Learning a globally applicable deep neural network (Lanaras 2018)](http://arxiv.org/abs/1803.04271)
- #PAPER [Deep Distillation Recursive Network for Remote Sensing Imagery Super-Resolution (Jiang 2018)](https://www.mdpi.com/2072-4292/10/11/1700/htm)
- #PAPER [Super-Resolution of PROBA-V Images Using [[CNNs]] (Martens 2019)](http://arxiv.org/abs/1907.01821)
- #PAPER [Deep Learning for Multiple-Image Super-Resolution (Kawulok 2019)](https://arxiv.org/abs/1903.00440)
	- EvoNet employs a deep ResNet to enhance the capabilities of evolutionary imaging model (EvoIM) for multiple-image SRR
	- https://www.youtube.com/watch?v=_RFQP1rRusQ&list=PLvT7fd9OiI9XORxAfLw_f9CsDkvM9lfKs&index=18&t=0s
- #PAPER [Super-Resolution Restoration of MISR Images Using the UCL MAGiGAN System (Tao 2019)](https://www.mdpi.com/2072-4292/11/1/52/htm)
- #PAPER [A Multi-Scale Wavelet 3D-CNN for Hyperspectral Image Super-Resolution (Yang 2019)](https://www.mdpi.com/2072-4292/11/13/1557/htm)
- #PAPER [Ultra-dense [[GANs]] for satellite imagery super-resolution (2020)](https://www.sciencedirect.com/science/article/abs/pii/S0925231219314602)
- #PAPER [Super-resolution of multispectral satellite images using convolutional neural networks (Muller 2020)](https://arxiv.org/abs/2002.00580)
- #PAPER [DeepSUM: Deep neural network for Super-resolution of Unregistered Multitemporal images (Bordone Molini 2020)](https://arxiv.org/abs/1907.06490)
	- Winner of the PROBA-V super-resolution challenge issued by the European Space Agency
	- #CODE https://github.com/diegovalsesia/deepsum
- #PAPER [DeepSUM++: Non-local Deep Neural Network for Super-Resolution of Unregistered Multitemporal Images  (Bordone Molini 2020)](https://arxiv.org/abs/2001.06342)
- #PAPER [D-SRGAN: DEM Super-Resolution with [[GANs]] (Demiray 2020)](https://arxiv.org/abs/2004.04788)
- #PAPER [Super-Resolution of Sentinel-2 Imagery Using Generative Adversarial Networks (Salgueiro Romero 2020)](https://www.mdpi.com/2072-4292/12/15/2424/htm)
	- https://upcommons.upc.edu/bitstream/handle/2117/329711/Final_thesis_OEC.pdf


### Data Fusion
- #PAPER [The SEN1-2 Dataset for [[AI/Deep learning/DL]] in SAR-Optical Data Fusion (Schmitt 2018)](http://arxiv.org/abs/1807.01569)
- #PAPER [Urban big data fusion based on deep learning: An overview (Liu 2020)](https://www.sciencedirect.com/science/article/pii/S1566253519301393)


### Data and benchmark datasets
See [[AI4ES/AI4ES data#EO and Satellite data]]




