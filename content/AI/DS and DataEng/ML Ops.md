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

## Courses
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
- [Azure (Microsoft)](https://azure.microsoft.com/en-gb/)
	- [Azure ML Studio](https://azure.microsoft.com/en-us/services/machine-learning/)
	- [Microsoft Cognitive Services](https://azure.microsoft.com/en-in/services/cognitive-services/)
- [Google Cloud Platform](https://cloud.google.com/)
	- [Vertex AI](https://cloud.google.com/vertex-ai) - Google Cloud’s unified ML platform
		- [Take your ML models from prototype to production with Vertex AI](https://cloud.google.com/blog/products/ai-machine-learning/go-from-a-notebook-to-a-production-ml-model)
	- [Pick your AI/ML Path on Google Cloud](https://cloud.google.com/blog/topics/developers-practitioners/pick-your-aiml-path-google-cloud)
	- https://codelabs.developers.google.com/
	- https://cloud.google.com/products/ai/
	- https://medium.com/google-cloud/jupyter-tensorflow-nvidia-gpu-docker-google-compute-engine-4a146f085f17
	- [Cloud AI building blocks](https://cloud.google.com/products/ai/building-blocks/)
	- [Cloud ML Engine](https://cloud.google.com/ml/)
		- [Google Cloud Machine Learning platform](https://cloud.google.com/ml-engine/docs/)
		- #TALK [Machine Intelligence at Google Scale: Vision/Speech API (Guillaume Laforge)](https://www.youtube.com/watch?v=zqWt8oI4gEw)
		- https://www.slideshare.net/matthiasfeys/machine-learning-at-scale-with-google-cloud-platform
		- https://github.com/Fematich/mlengine-boilerplate
	- [AI Hub](https://cloud.google.com/ai-hub/)
	- [Cloud AutoML](https://cloud.google.com/automl/)
- [Amazon web services (AWS)](https://aws.amazon.com/)
	- https://github.com/donnemartin/awesome-aws
	- [ML on AWS](https://aws.amazon.com/machine-learning/)
	- [SageMaker](https://aws.amazon.com/sagemaker/)
	- [AI on AWS](https://aws.amazon.com/lex/) 
		- https://aws.amazon.com/polly
		- https://aws.amazon.com/rekognition
- [Watson (IBM)](http://www.ibm.com/watson/)
	- [IBM Watson APIs](https://www.ibm.com/watson/developer/)
	- http://www.datasciencecentral.com/profiles/blogs/ibm-watson-does-your-taxes-question-answering-machine-versus-expe
	- https://www.codecademy.com/learn/ibm-watson
	- https://www.ibm.com/cloud/watson-studio
	- https://www.ibm.com/watson/services/knowledge-studio/
- [Dataiku DSS](https://www.dataiku.com/)
- [Domino DataLab](https://www.dominodatalab.com/)
- [RapidMiner](https://rapidminer.com/)
- [Knime](https://www.knime.org/knime-analytics-platform)
