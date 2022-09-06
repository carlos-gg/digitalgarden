---
title: "HPC-AI convergence"
---

> See:
> - [[AI4ES/AI4ES data]]
> - [[AI4ES/Pangeo]]

## Resources
- #TALK [Innovator Insights: HW & SW Platforms for HPC, AI and ML](https://www.youtube.com/watch?v=g4gNb5sEqyM)
- #TALK [HPC + AI: Machine Learning Models in Scientific Computing](https://www.youtube.com/watch?time_continue=1&v=SV3cnWf39kc&feature=emb_title)
	- https://es.slideshare.net/insideHPC/hpc-ai-machine-learning-models-in-scientific-computing

- The increasing interest in the usage of [[AI/Machine Learning]] (ML) and Artificial Intelligence techniques ([[AI/AI]]) to tackle high-impact research problems requires High Performance Computing (HPC) resources to efficiently compute and scale complex algorithms across thousands of nodes (Brayford et al. 2019). A diverse group of disciplines could be impacted by the integration of HPC and AI, especially those dealing with massive quantities of multi-dimensional data such as high energy physics, astrophysics and medical imaging.  
- The Barcelona Supercomputing Center (BSC), is in a privileged position for developing an AI centered research strategy thanks to, not only its vast expertise with HPC and running one of the largest supercomputers in Europe (the MareNostrum 4), but to the diverse and rich network of Machine Learning projects spread among its several departments. In particular, for the Earth Science department, it is of critical importance the extraction of knowledge from PB-sized databases coming from observations, numerical modeling, simulations, and other sources. 

### HPC vs AI programming models 
- One of the main challenges in the convergence of HPC and AI is the gap between programming models. 
- The worlds of HPC and AI deal with different computing paradigms or programming models. On one hand, for HPC it is the norm to use well tested and closed source code written in low-level languages (C, Fortran), distributed computing API's (MPI, OpenMPI), the command line and workload managers (SLURM), and systems that grant users restricted administrator privileges (no connection to external systems). On the other, in ML/AI fields the applications are usually developed using high-level scripting languages or frameworks (Python, Julia, Tensorflow) that usually address the challenges of writing performant and distributed code, and heavily relying on open source libraries which need to be downloaded from external sources (internet). The way ML applications are developed requires an interactive computing platform where new models could be tested and validated quickly without the overhead of restrictive administrative rules (very often related to security measures).The interactive computing paradigm implies code development, real-time exploratory data analytics, and visualizations of inputs and results. The design of ML models, opposed to calling pre-coded numerical models, requires a lot of experimentation.  
- The most recent family of ML algorithms, based on deep neural networks (Deep Learning, DL), has become the workhorse of AI. In order to handle complex problems, DL relies on training increasingly bigger deep networks on large amounts of data, which usually make use of specialized hardware, such as Graphical Processing Units (GPU).  

### Interactive computing and containers 
- [[AI/DS and DataEng/Data Science]] and ML require interactive/exploratory computing platforms and more flexible environments that allow on-the-fly software stack modifications (the installation of new libraries) and reproducibility of these software stacks. For Python this could be achieved with Pipenv or Conda (without sudo). However, a more general solution is to use containers, which are a combination of Kernel "cgroups" and "namespaces" to create isolated environments. Docker provided a complete tool chain to simplify using containers from build to run. Containers address a few of the aspects described before, which are very relevant to modern scientific computing: reusability, collaboration, reproducibility and portability.  Unfortunately, some of the characteristics of Docker prevent from it being in HPC systems:  
	- Uses an all or nothing security model, which would grant users with system privilege. 
	- It does not play well with batch systems, 
	- Assumes a local disk. 
	- Requires a very modern kernel. 
	- Its adoption would imply adding new layers of complexity to the HPC systems. 
- In order to deal with the security and integration issues of Docker, several HPC container systems were created. Usually these container solutions are backwards compatible with Docker, and among them the most widespread and mature are: 
	- [Shifter](https://github.com/NERSC/shifter) 
		- developed at NERSC to enable Docker images to be securely executed on a HPC ecosystem, enabling user independence, shared resource availability and high security1
	- [Singularity](https://github.com/sylabs/singularity)
		- very popular container used in many supercomputing centers, with a similar runtime compared to Shifter
	- [Charliecloud](https://github.com/hpc/charliecloud)
		- light-weight container system developed at LANL with high standards of security

#### Talks
- #TALK [Reproducible Science with Containers on HPC through Singularity](https://insidehpc.com/2019/02/video-reproducible-science-with-containers-on-hpc-through-singularity/)
- #TALK Containers in HPC. IDEAS webinar by Shane Canon 
	- http://ideas-productivity.org/wordpress/wp-content/uploads/2019/02/webinar026-containers.pdf 
	- https://www.youtube.com/watch?v=vzHnIS-bQQY 
- #TALK [Distributed HPC Applications with Unprivileged Containers](https://insidehpc.com/2020/02/distributed-hpc-applications-with-unprivileged-containers/)
- Container technologies:

### Jupyter project 
See [[AI/DS and DataEng/Jupyter#Jupyter in HPC]]
- The goal of this short text is to propose solutions in order to close the gap between the programming models of HPC and AI. These solutions are based on a review of the developments done in other supercomputing centers around the world. The idea is to share this text with Kim and Paco, to hopefully motivate future discussions with the Operations department.


## References
- #PAPER [The Convergence of AI and HPC](https://www.intel.com/content/www/es/es/high-performance-computing/ai-hpc-is-happening-now-report.html)
- #PAPER [Convergence of HPC and AI: 2 directions of connection (Ismayilova 2018)](http://azjhpc.org/issua2/doi.org:10.32010:26166127.2018.1.2.179.184.pdf)
- #PAPER [Deploying AI Frameworks on Secure HPC Systems with Containers (Brayford 2019)](https://arxiv.org/abs/1905.10090)



 