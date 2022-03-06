# Jupyter
- #CODE Jupyter: https://github.com/jupyter
	- #CODE Jupyterlab: https://github.com/jupyterlab/jupyterlab 
	- #CODE Jupyter(hub): https://jupyter.org/hub 
	- #CODE Jupyterlite: https://github.com/jupyterlite
		- https://blog.jupyter.org/jupyterlite-jupyter-%EF%B8%8F-webassembly-%EF%B8%8F-python-f6e2e41ab3fa
- #CODE Papermill - Parameterize, execute, and analyze notebooks: https://github.com/nteract/papermill

- Books with Jupyter: https://jupyterbook.org/intro.html
- [Executing notebooks from the command line](https://nbconvert.readthedocs.io/en/latest/execute_api.html#executing-notebooks-from-the-command-line "Permalink to this headline")
	- `$ jupyter nbconvert --to notebook --inplace --ExecutePreprocessor.timeout=None --execute mynotebook.ipynb`

## Jupyter in HPC
- High-level scripting languages such as Python, R and Julia, have become the go-to choices in the world of Data Science and ML/AI. Project Jupyter exists to develop open-source software, open-standards, and services for interactive computing across dozens of programming languages. For instance, the Jupyter Notebook is an open-source web-app that allows users to write portable documents containing executable code, narrative text, and equations, and to visualize the results of running the code directly in the web browser. The name comes from a combination of the three core programming languages of Jupyter (Julia, Python and R) though Jupyter is not limited to these languages.  
- Tools in the Jupyter ecosystem are designed in a modular fashion, and behave similarly on a researcher's laptop, a high-performance computing center, or the cloud. As a result, Jupyter technologies have been widely adopted across a spectrum of scientific disciplines, including Earth Sciences (Perez et al. 2019).  
- JupyterHub brings the power of notebooks to groups of users. It gives users access to computational environments and resources without burdening the users with installation and maintenance tasks. These are a few examples of JupyterHub systems running on supercomputing systems: 
	- University Corporation for Atmospheric Research (UCAR, https://jupyterhub.ucar.edu/)  
	- CSCS, ETH Zurich (https://jupyter.cscs.ch/hub/login) 
	- CHPC, University of Utah (https://www.chpc.utah.edu/documentation/software/jupyterhub.php#hub, http://notebook.chpc.utah.edu/) 
	- Minesota supercomputing institute (https://www.msi.umn.edu/content/msi-beta) 
- A common denominator of these computing platforms is that they allow the interactive execution of Jupyter tools on HPC systems over multiple nodes. The user is offered to choose the job configuration options in order to allocate the resources to be used to run Jupyter: account, number of nodes, access to GPUs, wall-clock time, etc.  
- Interactive supercomputing with Jupyter lab: https://www.cscs.ch/publications/news/2019/interactive-supercomputing-with-jupyterlab/

- #PAPER Jupyter as common technology platform for interactive HPC services (Milligan 2018): https://arxiv.org/abs/1807.09929
- #PAPER Jupyter meets the Earth: Enabling discovery in geoscience through interactive computing at scale (Perez 2019): https://zenodo.org/record/3369939 
- #PAPER Interactive Supercomputing with Jupyter (Thomas 2021): https://authorea.com/doi/full/10.22541/au.161230518.84458221 ^thomas21hpcjupyter


## Ipython
- Save interactive ipython session: `%history -f /tmp/history.py`
