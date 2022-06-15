---
title: "Pangeo"
---

## Resources
- Pangeo - A community platform for Big Data geoscience: https://pangeo.io/
- https://github.com/pangeo-data/education-material
- https://github.com/pangeo-data/awesome-open-climate-science
- https://github.com/pangeo-data/ml-workflow-examples
- https://github.com/pangeo-data/
- https://discourse.pangeo.io/


## Code
- #CODE Pangeo: https://github.com/pangeo-data
- #CODE Rechunker - Disk-to-disk chunk transformation for chunked arrays: https://github.com/pangeo-data/rechunker
	- https://rechunker.readthedocs.io/en/latest/
- #CODE Climpred - Verification of weather and climate forecasts: https://github.com/pangeo-data/climpred
	- https://climpred.readthedocs.io/en/stable/index.html
	- Metrics for forecast verification: https://climpred.readthedocs.io/en/stable/metrics.html
- #CODE xESMF: Universal Regridder for Geospatial Data: https://github.com/pangeo-data/xESMF
	- https://pangeo-xesmf.readthedocs.io/en/latest/
	- Comparison of 5 regridding algorithms: https://xesmf.readthedocs.io/en/latest/notebooks/Compare_algorithms.html


## References
### Pangeo for HPC
- Pangeo for DL: https://github.com/pangeo-data/pangeo/issues/567
- Streaming with Zarr: https://medium.com/pangeo/streaming-zarr-ccf0d518b1c0

-   #PAPER The PANGEO Big Data Ecosystem and its use at CNES (Eynard-Bontemps 2019): https://oceanrep.geomar.de/45866/
    -   https://medium.com/pangeo/why-and-how-we-use-pangeo-at-cnes-74553c7fb19b
-   #PAPER The Pangeo Ecosystem: Interactive Computing Tools for the Geosciences: Benchmarking on HPC (Odaka 2019): https://www.springerprofessional.de/en/the-pangeo-ecosystem-interactive-computing-tools-for-the-geoscie/17832674
    -   https://archimer.ifremer.fr/doc/00597/70946/
    -   #CODE https://github.com/pangeo-data/benchmarking


### Dask
See [[AI/DS and DataEng/Dask]]
```python
    # For the dask dashboard
	from dask.distributed import Client
	client = Client()
	display(client)
``` 

### Xarray
See [[AI/DS and DataEng/Xarray]]
- https://medium.com/pangeo/thoughts-on-the-state-of-xarray-within-the-broader-scientific-python-ecosystem-5cee3c59cd2b
- Slow performance of open_mfdataset: https://github.com/pydata/xarray/issues/1385
	- https://xarray.pydata.org/en/stable/io.html#reading-multi-file-datasets


### Jupyter
See [[AI/DS and DataEng/Jupyter]]


