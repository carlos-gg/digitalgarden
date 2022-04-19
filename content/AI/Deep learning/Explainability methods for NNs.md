---
title: "Explainability methods for NNs"
---

## Resources 
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

### Saliency maps
- https://en.wikipedia.org/wiki/Saliency_map
- Saliency map is a broader term from the field of computer vision. The first reference of saliency maps applied to the predictions of DNNs is Morch et al 1995. Simonyan et al (2014) first proposed a method to produce saliency maps using back-propagation through a CNN, but note that you could compute "saliency" from an image in many ways that do not deal with back-propagating the prediction scores of DNNs. 
- [Pixel Attribution (Saliency Maps)](https://christophm.github.io/interpretable-ml-book/pixel-attribution.html)

### Layer-wise Relevance Propagation (LRP)
- LRP is an inverse method which calculates the contribution of a single pixel to the prediction made by a DNN in an image classification task
- http://heatmapping.org/
- [Interactive demo](https://lrpserver.hhi.fraunhofer.de/image-classification)
- https://medium.com/@ODSC/layer-wise-relevance-propagation-means-more-interpretable-deep-learning-219ff5158914
- https://towardsdatascience.com/indepth-layer-wise-relevance-propagation-340f95deb1ea
- There are several approaches for calculating attributions by back-propagating the prediction score through each layer of the network, back to the input features /pixels (DeConvNet, SmoothGrad, GradCam, LRP, XRAI). LRP is just one of them. In the first LRP paper, they talk about heatmaps or relevance maps, probably to avoid confusion with older saliency map techniques


## Courses
- #COURSE [Interpretable Machine Learning for Computer Vision (CVPR 2020)](https://interpretablevision.github.io/index_cvpr2020.html)
- #COURSE [Explainability Methods for Neural Networks (2021)](https://sites.google.com/view/emnn-ws-2020/home)


## Code
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
	- #CODE See Code section
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
- #PAPER [Explaining in Style: Training a GAN to explain a classifier in StyleSpace (Lang 2021)](https://explaining-in-style.github.io/)
	- https://ai.googleblog.com/2022/01/introducing-stylex-new-approach-for.html

 
### Layer-wise Relevance Propagation (LRP)
- #PAPER [On Pixel-Wise Explanations for Non-Linear Classifier Decisions by Layer-Wise Relevance Propagation (Bach 2015)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0130140)
	- #CODE [Tutorial: Implementing Layer-Wise Relevance Propagation](https://git.tu-berlin.de/gmontavon/lrp-tutorial)
- #PAPER [Understanding Individual Decisions of CNNs via Contrastive Backpropagation (Gu 2019)](https://arxiv.org/abs/1812.02100)
- #PAPER [Beyond saliency: understanding convolutional neural networks from saliency prediction on layer-wise relevance propagation (Li 2019)](https://arxiv.org/abs/1712.08268)
	- proposed a novel two-step understanding method, namely Salient Relevance (SR) map, which aims to shed light on how deep CNNs recognize images and learn features from attention areas
	- starts out with a layer-wise relevance propagation (LRP) step which estimates a pixel-wise relevance map over the input image. Following, we construct a context-aware saliency map, SR map, from the LRP-generated map which predicts areas close to the foci of attention instead of isolated pixels that LRP reveals
- #PAPER [Towards Best Practice in Explaining Neural Network Decisions with LRP (Kohlbrenner 2020)](https://arxiv.org/abs/1910.09840)
