---
title: "XAI"
disableToc: false 
---

## Resources
- Explainable AI (XAI), or Interpretable AI, is artificial intelligence (AI) in which the results of the solution can be understood by humans
- https://en.wikipedia.org/wiki/Explainable_artificial_intelligence
- https://github.com/anguyen8/XAI-papers
- [Ideas on interpreting machine learning](https://www.oreilly.com/ideas/ideas-on-interpreting-machine-learning)
- [Explainable AI demos](https://lrpserver.hhi.fraunhofer.de/)
- [Why you need to care about Explainable Machine Learning](https://medium.com/james-blogs/why-you-need-to-care-about-explainable-machine-learning-d01196a6af76)
- [Interpreting machine learning models](https://towardsdatascience.com/interpretability-in-machine-learning-70c30694a05f)
- [I.am.ai. Explaining artificial intelligence](https://www.i-am.ai/)
- [Baking recipes made by AI](https://cloud.google.com/blog/topics/developers-practitioners/baking-recipes-made-ai)
- A Review of Different Interpretation Methods:
	- https://mrsalehi.medium.com/a-review-of-different-interpretation-methods-in-deep-learning-part-1-saliency-map-cam-grad-cam-3a34476bc24d
	- https://mrsalehi.medium.com/a-review-of-different-interpretation-methods-in-deep-learning-part-2-input-gradient-layerwise-e077609b6377
	- https://mrsalehi.medium.com/a-review-of-different-interpretation-methods-in-deep-learning-part-3-shap-integrated-gradients-918fc9fedd9b


## Events, talks
- [Workshop on Visualization for AI Explainability](http://visxai.io/)
- [ACM Conference on Fairness, Accountability, and Transparency](https://facctconference.org/)
- [Explainable AI xAI 2020](https://human-centered.ai/explainable-ai-2020/)
- #TALK [Synthesizing Explainable and Deceptive Behavior for Human-AI Interaction (AAAI 2020 Tutorial)](https://yochan-lab.github.io/tutorial/AAAI-2020/)
	- https://www.youtube.com/watch?v=r6KhJ3ORYnc
- #TALK [Explainable AI in Industry (Tutorial)](https://sites.google.com/view/explainable-ai-tutorial)
	- https://www.youtube.com/watch?list=PLewjn-vrZ7d3x0M4Uu_57oaJPRXkiS221&v=rcUw7PXHWF4
- #TALK [Explainable AI: Foundations, Industrial Applications, Practical Challenges, and Lessons Learned (AAAI 2020)](https://xaitutorial2020.github.io/)
	- https://xaitutorial2020.github.io/raw/master/slides/aaai_2020_xai_tutorial.pdf


## Books
- #BOOK [ Interpretable Machine Learning (Molnar 2021)](https://christophm.github.io/interpretable-ml-book/)


## Code
- https://towardsdatascience.com/explainable-ai-xai-a-guide-to-7-packages-in-python-to-explain-your-models-932967f0634b

- #CODE [CARLA](https://github.com/carla-recourse/CARLA)
	- CARLA is a python library to benchmark counterfactual explanation and recourse models
	- #PAPER [CARLA: A Python Library to Benchmark Algorithmic Recourse and Counterfactual Explanation Algorithms (Pawelczyk 2021)](https://arxiv.org/abs/2108.00783)
	- https://www.marktechpost.com/2021/08/22/university-of-tubingen-researchers-open-source-carla-a-python-library-for-benchmarking-counterfactual-explanation-methods-across-data-sets-and-machine-learning-models/
- #CODE [Shapash](https://github.com/MAIF/shapash)
	- https://shapash.readthedocs.io/en/latest/
- #CODE [ExplainerDashboard](https://github.com/oegedijk/explainerdashboard)
	- https://explainerdashboard.readthedocs.io/en/latest/index.html#
	- library for quickly building interactive dashboards for analyzing and explaining the predictions and workings of (scikit-learn compatible) machine learning models, including xgboost, catboost and lightgbm
	- #TALK https://www.youtube.com/watch?v=1nMlfrDvwc8
- #CODE [AIX360](https://github.com/Trusted-AI/AIX360) ^aix360
	- Interpretability and explainability of data and machine learning models
	- http://aix360.mybluemix.net/
- #CODE [LIME: Local Interpretable Model-agnostic Explanations](https://github.com/marcotcr/lime) ^limegithub
- #CODE [Skater](https://github.com/datascienceinc/Skater)
	- Skater is a python package for model agnostic interpretation of predictive models. With Skater, you can unpack the internal mechanics of arbitrary models; as long as you can obtain inputs, and use a function to obtain outputs, you can use Skater to learn about the models internal decision policies.
	- https://datascienceinc.github.io/Skater/overview.html
	- Understanding How and Why Your Model Works:  https://www.datascience.com/learn-data-science/fundamentals/model-interpretation-algorithms
	- https://www.datascience.com/resources/tools/skater
- #CODE [FairML - Auditing Black-Box Predictive Models](https://github.com/adebayoj/fairml)
	- FairML is a python toolbox auditing the machine learning models for bias. 
	- http://blog.fastforwardlabs.com/2017/03/09/fairml-auditing-black-box-predictive-models.html
- #CODE [ELI5](https://github.com/TeamHG-Memex/eli5)
	- ELI5 is a Python library which allows to visualize and debug various Machine Learning models using unified API. It has built-in support for several ML frameworks and provides a way to explain black-box models.
	- http://eli5.readthedocs.io/en/latest/
- #CODE [BlackBox Auditing](https://github.com/algofairness/BlackBoxAuditing)
- #CODE [SHAP](https://github.com/slundberg/shap) ^shapgithub
	- Unified approach to explain the output of any machine learning model. SHAP connects game theory with local explanations, uniting several previous methods and representing the only possible consistent and locally accurate additive feature attribution method based on expectations.
- #CODE [InterpretML - Microsoft open-source package that incorporates state-of-the-art machine learning interpretability techniques under one roof](https://github.com/interpretml/interpret)
- #CODE [uncertainty-toolbox](https://github.com/uncertainty-toolbox/uncertainty-toolboxç)
- #CODE [imodels](https://github.com/csinva/imodels)
	- Python package for concise, transparent, and accurate predictive modeling. All sklearn-compatible and easy to use.

### Deep NNs XAI
- #CODE [Quantus](https://github.com/understandable-machine-intelligence-lab/Quantus)
	- Quantus is an eXplainable AI toolkit for responsible evaluation of neural network explanations
- #CODE [TruLens (tf.keras and pytorch): Explainability for Neural Networks](https://github.com/truera/trulens)
	- https://www.trulens.org/
- #CODE [Captum (pytorch)](https://github.com/pytorch/captum)
	- Interpretability of models across modalities including vision, text, and more
	- https://captum.ai/
	- https://captum.ai/api/
- #CODE [Saliency](https://github.com/PAIR-code/saliency)
	- XRAI, SmoothGrad, Vanilla Gradients, Guided Backpropogation, Integrated Gradients, Occlusion, Grad-CAM, Blur IG
- #CODE [iNNvestigate](https://github.com/albermax/innvestigate) ^innvestigate
	- Vanilla gradient, SmoothGrad, DeConvNet, Guided BackProp, PatternNet, DeepTaylor, PatternAttribution, LRP, IntegratedGradients, DeepLIFT
- #CODE [TF-explain](https://github.com/sicara/tf-explain)
	- implements interpretability methods as Tensorflow 2.x callbacks to ease neural network's understanding
- #CODE [TensorSpace (Tensorflow.js)](https://github.com/tensorspace-team/tensorspace)
	- Neural network 3D visualization framework
	- https://tensorspace.org
- #CODE [Lucid (Tensorflow 1) - A collection of infrastructure and tools for research in neural network interpretability](https://github.com/tensorflow/lucid)
- #CODE [tf-keras-vis](https://github.com/keisen/tf-keras-vis)
	- Neural network visualization toolkit for tf.keras
	- Activation Maximization
	- Class Activation Maps (GradCAM, GradCAM++, ScoreCAM, Faster-ScoreCAM)
	- Saliency Maps (Vanilla Saliency, SmoothGrad)
- #CODE [Keras-vis](https://github.com/raghakot/keras-vis)
	- https://raghakot.github.io/keras-vis/
	- Activation maximization, Saliency maps, Class activation maps
- #CODE [DeepExplain (TensorFlow 1)](https://github.com/marcoancona/DeepExplain)
	- Saliency maps, Gradient * Input, Integrated Gradients, DeepLIFT, ε-LRP
- #CODE [LRP toolbox](https://github.com/sebastian-lapuschkin/lrp_toolbox)


## References
- #PAPER [The Mythos of Model Interpretability (Lipton 2017)](https://arxiv.org/abs/1606.03490)
- #PAPER [A Survey of Methods for Explaining Black Box Models (Guidotti, 2018)](https://dl.acm.org/doi/10.1145/3236009)
- #PAPER [Making the Black Box More Transparent: Understanding the Physical Implications of Machine Learning (McGovern et al. 2019)](https://journals.ametsoc.org/bams/article/100/11/2175/343787/Making-the-Black-Box-More-Transparent)
- #PAPER [Towards Explainable Artificial Intelligence (Samek & Muller 2019)](https://arxiv.org/abs/1909.12072)
- #PAPER [Explaining Explanations: An Overview of Interpretability of Machine Learning (Gilpin et al. 2019)](https://arxiv.org/abs/1806.00069)
- #PAPER [One Explanation Does Not Fit All: A Toolkit and Taxonomy of AI Explainability Techniques (Arya 2019)](https://arxiv.org/abs/1909.03012)
	- #CODE [[#^aix360]]
- #PAPER [Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead (Rudin 2019)](https://www.nature.com/articles/s42256-019-0048-x)
	- https://arxiv.org/abs/1811.10154
- #PAPER [Explainable Machine Learning for Scientific Insights and Discoveries (Roscher 2020)](https://arxiv.org/abs/1905.08883)
- #PAPER [Review Study of Interpretation Methods for Future Interpretable Machine Learning (Jian-Xun 2020)](https://ieeexplore.ieee.org/document/9234594)

### Model-agnostic methods
- https://christophm.github.io/interpretable-ml-book/agnostic.html
	- The great advantage of model-agnostic interpretation methods over model-specific ones is their flexibility
	- An alternative to model-agnostic interpretation methods is to use only interpretable models, which often has the big disadvantage that predictive performance is lost compared to other machine learning models and you limit yourself to one type of model
- #PAPER [Model-Agnostic Interpretability of Machine Learning (Tulio Ribeiro 2016)](https://arxiv.org/abs/1606.05386)
- #PAPER [SHAP - A Unified Approach to Interpreting Model Predictions (Lundberg 2017)](https://arxiv.org/abs/1705.07874)
	- SHAP (SHapley Additive exPlanations)
	- #CODE [[#^shapgithub]]
	- Can be used for computer vision tasks

- #PAPER [Peeking Inside the Black Box: Visualizing Statistical Learning With Plots of Individual Conditional Expectation (Goldstein 2014)](https://arxiv.org/abs/1309.6392)

#### Partial Dependence Plot
- The partial dependence plot (short PDP or PD plot) shows the marginal effect one or two features have on the predicted outcome of a machine learning model
- https://christophm.github.io/interpretable-ml-book/pdp.html
- https://scikit-learn.org/stable/modules/partial_dependence.html

#### Individual Conditional Expectation
- Individual Conditional Expectation (ICE) plots display one line per instance that shows how the instance's prediction changes when a feature changes
- https://christophm.github.io/interpretable-ml-book/ice.html
- https://scikit-learn.org/stable/modules/partial_dependence.html

#### Permutation Feature Importance
- Permutation feature importance measures the increase in the prediction error of the model after we permuted the feature's values, which breaks the relationship between the feature and the true outcome
- https://christophm.github.io/interpretable-ml-book/feature-importance.html
- https://scikit-learn.org/stable/modules/permutation_importance.html
	- The permutation feature importance is defined to be the decrease in a model score when a single feature value is randomly shuffled
	- Tree-based models provide an alternative measure of feature importances based on the mean decrease in impurity (MDI). Impurity is quantified by the splitting criterion of the decision trees (Gini, Entropy or Mean Squared Error). However, this method can give high importance to features that may not be predictive on unseen data when the model is overfitting. Permutation-based feature importance, on the other hand, avoids this issue, since it can be computed on unseen data

#### Surrogate models
- A surrogate model is a simple model that is used to explain a complex model. Surrogate models are usually created by training a linear regression or decision tree on the original inputs and predictions of a complex model. Coefficients, variable importance, trends, and interactions displayed in the surrogate model are then assumed to be indicative of the internal mechanisms of the complex model. There are few, possibly no, theoretical guarantees that the simple surrogate model is highly representative of the more complex model.
- The globally interpretable attributes of a simple model are used to explain global attributes of a more complex model. However, there is nothing to preclude fitting surrogate models to more local regions of a complex model's conditional distribution, such as clusters of input records and their corresponding predictions and their corresponding input rows. Because small sections of the conditional distribution are more likely to be linear, monotonic, or otherwise well-behaved, local surrogate models can be more accurate than global surrogate models.
- #PAPER [LIME - "Why Should I Trust You?": Explaining the Predictions of Any Classifier (2016)](https://arxiv.org/abs/1602.04938) ^lime
	- #CODE [[#^limegithub]]
	- Formalized approach for local surrogate models. It is meant to shed light on how decisions are made for specific observations. LIME requires that a set of explainable records be found, simulated, or created.
	- https://www.oreilly.com/learning/introduction-to-local-interpretable-model-agnostic-explanations-lime
	- https://github.com/albahnsen/Talk_Demystifying_Machine_Learning
	- [Interpreting ML models prediction power](http://www.datasciencecentral.com/profiles/blogs/deep-learning-epic-fail-right-answer-wrong-reason)
	- https://medium.com/@ageitgey/natural-language-processing-is-fun-part-3-explaining-model-predictions-486d8616813c
	- Machine Learning Explained - Easysol:  http://blog.easysol.net/machine_learning_explained/
	- https://www.slideshare.net/albahnsen/demystifying-machine-learning-using-lime
	- https://github.com/albahnsen/Talk_Demystifying_Machine_Learning


### Maximum activation analysis
- See [Neural Networks explainability](#Neural%20Networks%20explainability)
- In maximum activation analysis, examples are found or simulated that maximally activate certain neurons, layers, or filters in a neural network or certain trees in decision tree ensembles. For the purposes of maximum activation analysis, low residuals for a certain tree are analogous to high-magnitude neuron output in a neural network.
- Maximum activation analysis elucidates internal mechanisms of complex models by determining the parts of the response function that specific observations or groups of similar observations excite to the highest degree, either by high-magnitude output from neurons or by low residual output from trees.


### Sensitivity analysis
- See [Neural Networks explainability](#Neural%20Networks%20explainability)
- Sensitivity analysis investigates whether model behavior and outputs remain stable when data is intentionally perturbed or other changes are simulated in data. 
- Beyond traditional assessment practices, sensitivity analysis of machine learning model predictions is perhaps the most important validation technique for machine learning models. 
- Machine learning models can make drastically differing predictions from minor changes in input variable values. In practice, many linear model validation techniques focus on the numerical instability of regression parameters due to correlation between input variables or between input variables and the dependent variable
- Sensitivity analysis can also test model behavior and outputs when interesting situations or known corner cases are simulated. Output distributions, error measurements, plots, and interpretation techniques can be used to explore the way models behave in important scenarios, how they change over time, or if models remain stable when data is subtly and intentionally corrupted


### Variable importance measures
- Variable importance measures are typically seen in tree-based models but are sometimes also reported for other models.
- A simple heuristic rule for variable importance in a decision tree is related to the depth and frequency at which a variable is split on in a tree, where variables used higher in the tree and more frequently in the tree are more important. 
- For a single decision tree, a variable's importance is quantitatively determined by the cumulative change in the splitting criterion for every node in which that variable was chosen as the best splitting candidate. 
- For a gradient boosted tree ensemble, variable importance is calculated as it is for a single tree but aggregated for the ensemble. 
- For random forests:
	- Variable importance is also calculated as it is for a single tree and aggregated, but an additional measure of variable importance is provided by the change in out-of-bag accuracy caused by shuffling the independent variable of interest, where larger decreases in accuracy are taken as larger indications of importance
	- The default method to compute variable importance is the mean decrease in impurity (or gini importance) mechanism: At each split in each tree, the improvement in the split-criterion is the importance measure attributed to the splitting variable, and is accumulated over all the trees in the forest separately for each variable. Note that this measure is quite like the R^2 in regression on the training set
	- [This example highlights the limitations of impurity-based feature importance in contrast to permutation-based feature importance](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html)
	- #PAPER [Understanding variable importances in forests of randomized trees (Louppe 2013)](https://papers.nips.cc/paper/4928-understanding-variable-importances-in-forests-of-randomized-trees.pdf)
		- #POSTER https://orbi.uliege.be/bitstream/2268/155642/3/poster.pdf
	- #PAPER [Trees, forests, and impurity-based variable importance (Scornet 2020)](https://arxiv.org/abs/2001.04295)
- For neural networks, variable importance measures are typically associated with the aggregated, absolute magnitude of model parameters for a given variable of interest. 
- Global variable importance techniques are typically model specific, and practitioners should be aware that unsophisticated measures of variable importance can be biased toward larger scale variables or variables with a high number of categories.


### Neural Networks explainability
See [Code](#Code#Deep%20XAI)

#### Resources 
- [Using ML to Explore Neural Network Architecture](https://research.googleblog.com/2017/05/using-machine-learning-to-explore.html)
- [The Building Blocks of Interpretability](https://distill.pub/2018/building-blocks/)
- [Feature Visualization](https://distill.pub/2017/feature-visualization/)
- [Applying deep learning to real-world problems (labeled data, imbalance, black box models)](https://medium.com/merantix/applying-deep-learning-to-real-world-problems-ba2d86ac5837)
- [Unblackboxing webinar (deepsense.io)](https://github.com/deepsense-io/unblackboxing_webinar)
- [The Dark Secret at the Heart of AI](https://www.technologyreview.com/s/604087/the-dark-secret-at-the-heart-of-ai/amp/)
- [How AI detectives are cracking open the black box of deep learning](http://www.sciencemag.org/news/2017/07/how-ai-detectives-are-cracking-open-black-box-deep-learning)
- [Visualization of activations and filters](https://blog.keras.io/how-convolutional-neural-networks-see-the-world.html) 
	- https://github.com/jacobgil/keras-filter-visualization
- https://towardsdatascience.com/understanding-your-convolution-network-with-visualizations-a4883441533b
- https://imatge.upc.edu/web/publications/visual-saliency-prediction-using-deep-learning-techniques
- [Attributing a deep network’s prediction to its input features](http://www.unofficialgoogledatascience.com/2017/03/attributing-deep-networks-prediction-to.html)
	- Integrated gradients method
	- It involves a few calls to a gradient operator yielding insightful results for a variety of deep networks
- [Pixel Attribution (Saliency Maps)](https://christophm.github.io/interpretable-ml-book/pixel-attribution.html)

  
#### References
- #PAPER [Visualization of neural networks using saliency maps (Morch 1995)](https://www.researchgate.net/publication/3623243_Visualization_of_neural_networks_using_saliency_maps)
- #PAPER [Deep inside CNNs: Visualising Image Classification Models and Saliency Maps (Simonyan 2014)](https://arxiv.org/abs/1312.6034)
	- Presented two visualisation techniques for deep classification ConvNets
		- The first generates an artificial image, which is representative of a class of interest
		- The second computes an image-specific class saliency map, highlighting the areas of the given image, discriminative wrt the given class
- #PAPER [Understanding Neural Networks Through Deep Visualization (Yosinski 2015)](https://arxiv.org/abs/1506.06579)
	- http://yosinski.com/deepvis
- #PAPER [SVCCA: Singular Vector Canonical Correlation Analysis for Deep Learning Dynamics and Interpretability (Raghu 2017)](https://arxiv.org/abs/1706.05806)
	- [Interpreting Deep Neural Networks with SVCCA](https://ai.googleblog.com/2017/11/interpreting-deep-neural-networks-with.html)
- #PAPER [Axiomatic Attribution for Deep Networks (Sundararajan 2017)](https://arxiv.org/abs/1703.01365)
- #PAPER [SmoothGrad: removing noise by adding noise (Smilkov 2017)](https://arxiv.org/abs/1706.03825)
	- https://pair-code.github.io/saliency/
- #PAPER [iNNvestigate Neural Networks! (Alber 2018)](http://arxiv.org/abs/1808.04260)
	- #CODE [[#^innvestigate]]
- #PAPER [XRAI: Better Attributions Through Regions (Kapishnikov 2019)](https://arxiv.org/abs/1906.02825)
- #PAPER [DeepLIFT - Learning Important Features Through Propagating Activation Differences (Shrikumar 2019)](https://arxiv.org/abs/1704.02685)
 - #PAPER [Saliency Prediction in the Deep Learning Era: Successes, Limitations, and Future Challenges (Borji 2019)](https://arxiv.org/abs/1810.03716)
- #PAPER [DAX: Deep Argumentative eXplanation for Neural Networks (Albini 2020)](https://arxiv.org/abs/2012.05766)
- #PAPER [Interpreting Deep Neural Networks Through Variable Importance (Ish-Horowicz 2020)](https://arxiv.org/abs/1901.09839)
	- Their strategy is specifically designed to leverage partial covariance structures and incorporate variable interactions into our proposed feature ranking.  
	- Extended the recently proposed “RelATive cEntrality” (RATE) measure (Crawford et al., 2019) to the Bayesian deep learning setting
	- Given a trained network, RATE applies an information theoretic criterion to the posterior distribution of effect sizes to assess feature significance
- #PAPER [Determining the Relevance of Features for Deep Neural Networks (Reimers 2020)](https://link.springer.com/chapter/10.1007%2F978-3-030-58574-7_20)
	- Their approach builds upon concepts from causal inference
	- Interpret machine learning in a structural causal model and use Reichenbach’s common cause principle to infer whether a feature is relevant
- #PAPER [Explainable Deep Learning Models in Medical Image Analysis (Singh 2020)](https://arxiv.org/abs/2005.13799)
- #PAPER [Efficient Saliency Maps for Explainable AI (Mundhenk 2020)](https://arxiv.org/abs/1911.11293)
- #PAPER [Explaining Deep Neural Networks and Beyond: A Review of Methods and Applications (Samek 2021)](https://ieeexplore.ieee.org/document/9369420)
- #PAPER [Logic Explained Networks (Ciravegna 2021)](https://arxiv.org/abs/2108.05149)
	- https://syncedreview.com/2021/08/18/deepmind-podracer-tpu-based-rl-frameworks-deliver-exceptional-performance-at-low-cost-85/
- #PAPER [Toward Explainable AI for Regression Models (Letzgus 2021)](https://arxiv.org/abs/2112.11407)

 
##### Layer-wise Relevance Propagation (LRP)
- LRP is an inverse method which calculates the contribution of a single pixel to the prediction made by a DNN in an image classification task
- http://heatmapping.org/
- [Interactive demo](https://lrpserver.hhi.fraunhofer.de/image-classification)
- https://medium.com/@ODSC/layer-wise-relevance-propagation-means-more-interpretable-deep-learning-219ff5158914
- https://towardsdatascience.com/indepth-layer-wise-relevance-propagation-340f95deb1ea
- Saliency map is a broader term from the field of computer vision (https://en.wikipedia.org/wiki/Saliency\_map). The first reference of saliency maps applied to the predictions of DNNs is Morch et al 1995. Simonyan et al (2014) first proposed a method to produce saliency maps using back-propagation through a CNN, but note that you could compute "saliency" from an image in many ways that do not deal with back-propagating the prediction scores of DNNs. 
- There are several approaches for calculating attributions by back-propagating the prediction score through each layer of the network, back to the input features /pixels (DeConvNet, SmoothGrad, GradCam, LRP, XRAI). LRP is just one of them. In the first LRP paper, they talk about heatmaps or relevance maps, probably to avoid confusion with older saliency map techniques

- #PAPER [On Pixel-Wise Explanations for Non-Linear Classifier Decisions by Layer-Wise Relevance Propagation (Bach 2015)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0130140)
	- #CODE [Tutorial: Implementing Layer-Wise Relevance Propagation](https://git.tu-berlin.de/gmontavon/lrp-tutorial)
- #PAPER [Understanding Individual Decisions of CNNs via Contrastive Backpropagation (Gu 2019)](https://arxiv.org/abs/1812.02100)
- #PAPER [Beyond saliency: understanding convolutional neural networks from saliency prediction on layer-wise relevance propagation (Li 2019)](https://arxiv.org/abs/1712.08268)
	- proposed a novel two-step understanding method, namely Salient Relevance (SR) map, which aims to shed light on how deep CNNs recognize images and learn features from attention areas
	- starts out with a layer-wise relevance propagation (LRP) step which estimates a pixel-wise relevance map over the input image. Following, we construct a context-aware saliency map, SR map, from the LRP-generated map which predicts areas close to the foci of attention instead of isolated pixels that LRP reveals
- #PAPER [Towards Best Practice in Explaining Neural Network Decisions with LRP (Kohlbrenner 2020)](https://arxiv.org/abs/1910.09840)