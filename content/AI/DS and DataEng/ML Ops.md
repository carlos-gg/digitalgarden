---
title: "Machine Learning Operations (MLOps)"
---

> Set of practices that aims to deploy and maintain machine learning models in production reliably and efficiently. The word is a compound of "machine learning" and the continuous development practice of DevOps in the software field

## Resources
- https://en.wikipedia.org/wiki/MLOps
- https://github.com/GokuMohandas/MadeWithML
- https://github.com/visenger/awesome-mlops
- https://github.com/EthicalML/awesome-production-machine-learning
- [More Data, More Problems: Using DVC to handle data versioning for a computer vision problem](https://mlops.systems/tools/redactionmodel/computervision/mlops/2022/05/24/data-versioning-dvc.html)
- [What is MLOps and how to get started? | MLOps series](https://www.youtube.com/watch?v=LdLFJUlPa4Y)

## Courses
- #COURSE [Machine Learning Systems Design](https://stanford-cs329s.github.io/syllabus.html) (CS 329S, Stanford)
- #COURSE [Deploying Machine Learning Models in Production](https://www.coursera.org/learn/deploying-machine-learning-models-in-production) (Coursera, DeepLearning.AI)
- #COURSE [Effective MLOps - Model development](https://www.wandb.courses/courses/effective-mlops-model-development) (Weights & Biases)
- #COURSE [CI/CD for Machine Learning (GitOps)](https://www.wandb.courses/courses/ci-cd-for-machine-learning) (Weights & Biases)
- #COURSE [MLOps Course](https://github.com/GokuMohandas/mlops-course)
	- https://madewithml.com/#mlops

## Code
- #CODE [MUSE](https://github.com/Lightning-AI/stable-diffusion-deploy)
	- Open source, stable-diffusion production server to show how to deploy diffusion models in a real production environment with: load-balancing, gpu-inference, performance-testing, micro-services orchestration and more. All handled easily with the Lightning Apps framework

### Experiment tracking
- See [[AI/Supervised Learning/Model selection and tuning]]
- https://neptune.ai/blog/best-ml-experiment-tracking-tools
- #CODE [Weights & Biases](https://github.com/wandb/wandb) - A tool for visualizing and tracking your machine learning experiments
	- https://docs.wandb.com/
	- Tool to log hyperparameters and output metrics from your runs, then visualize and compare results and quickly share findings with your colleagues.
- #CODE [Aim](https://github.com/aimhubio/aim) - The open-source tool for ML experiment comparison
	- https://aimstack.io/
- #CODE [ClearML](https://github.com/allegroai/clearml)
	- https://clear.ml/

### Visualization and UI 
- #CODE [kedro-viz](https://github.com/kedro-org/kedro-viz) - Visualise your Kedro data and machine-learning pipelines and track your experiments
- #CODE [Gradio](https://github.com/gradio-app/gradio) - Create UIs for your machine learning model in Python in 3 minutes
	- https://gradio.app/

### Workflow managers
- #CODE [Kedro](https://github.com/kedro-org/kedro) - A Python framework for creating reproducible, maintainable and modular data science code
	- https://kedro.readthedocs.io/
- #CODE [MLrun](https://github.com/mlrun/mlrun) - The Open-Source MLOps Orchestration Framework
	- https://docs.mlrun.org/en/stable/
- #CODE [Metaflow](https://github.com/Netflix/metaflow) - Human-friendly Python/R library that helps scientists and engineers build and manage real-life data science projects
	- Originally developed at Netflix to boost productivity of data scientists who work on a wide variety of projects from classical statistics to state-of-the-art deep learning
	- https://metaflow.org/
	- #CODE [metaflow-ui](https://github.com/Netflix/metaflow-ui)
		- https://netflixtechblog.com/open-sourcing-a-monitoring-gui-for-metaflow-75ff465f0d60
- #CODE [Flyte](https://github.com/flyteorg/flyte) - Kubernetes-native workflow automation platform for complex, mission-critical data and ML processes at scale
	- It has been battle-tested at Lyft, Spotify, Freenome, and others and is truly open-source
	- https://flyte.org/
- #CODE [MLFlow](https://github.com/mlflow/mlflow/ )
	- [An open source platform for the machine learning lifecycle](https://mlflow.org)
- #CODE [Airflow](https://github.com/apache/airflow) - Apache Airflow is a platform to programmatically author, schedule, and monitor workflows
	- http://nerds.airbnb.com/airflow/
	- https://medium.com/datasd/why-data-automation-matters-4391d59e1952
- #CODE [Luigi (Spotify)](https://github.com/spotify/luigi)
	- https://luigi.readthedocs.io/en/latest/
- #CODE [Kubeflow](https://github.com/kubeflow/kubeflow) - cloud-native platform for machine learning operations - pipelines, training and deployment
	- https://www.kubeflow.org/
- #CODE [Azkaban](https://github.com/azkaban/azkaban)
- #CODE [PredictionIO (Apache)](https://predictionio.apache.org)

### ML platforms
See [[AI/DS and DataEng/Cloud platforms]]
