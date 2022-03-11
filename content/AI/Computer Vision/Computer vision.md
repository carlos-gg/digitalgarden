---
title: "Computer Vision"
disableToc: false 
---

See 
[CNNs](AI/Deep%20learning/CNNs.md)
[MLPs#MLPs for vision and language](AI/Deep%20learning/MLPs.md#MLPs%20for%20vision%20and%20language)
[Transformers#For Computer Vision](AI/Deep%20learning/Transformers.md#For%20Computer%20Vision.md)
[Generative modelling#Generative models for Image data](AI/Deep%20learning/Generative%20modelling.md#Generative%20models%20for%20Image%20data)
[GANs](AI/Deep%20learning/GANs.md)


## Resources
- https://github.com/jbhuang0604/awesome-computer-vision
- [Papers with code - computer vision](https://paperswithcode.com/area/computer-vision)

## Books
- #BOOK [Image Processing and Acquisition using Python (Chityala 2014)](https://www.crcpress.com/Image-Processing-and-Acquisition-using-Python/Chityala-Pudipeddi/p/book/9781466583757)
- #BOOK [Computer Vision: A Modern Approach (Forsyth, 2011 PEARSON)](https://www.pearson.com/us/higher-education/program/Forsyth-Computer-Vision-A-Modern-Approach-2nd-Edition/PGM111082.html)
	- https://github.com/yihui-he/computer-vision-tutorial/blob/master/Computer%20Vision%20A%20Modern%20Approach%202nd%20Edition.pdf
- #BOOK [Computer Vision: Models, Learning, and Inference (Prince, 2012 CAMBRIDGE)](http://www.computervisionmodels.com/)
- #BOOK [Computer vision (chapter)](https://d2l.ai/chapter_computer-vision/index.html)

## Courses
- #COURSE [Computer vision (CS543/ECE549, UIUC)](https://courses.engr.illinois.edu/cs543/sp2015/)
- #COURSE [Advances in Computer vision (MIT)](http://6.869.csail.mit.edu/fa18/)
- #COURSE [Introduction to computer vision (Udacity, Georgia Tech)](https://www.udacity.com/course/introduction-to-computer-vision--ud810)
- #COURSE [Deep Learning for Computer Vision (UPC TelecomBCN 2016)](http://imatge-upc.github.io/telecombcn-2016-dlcv/)
- #COURSE [Convolutional Neural Networks for Visual Recognition (CS231n, Stanford)](http://cs231n.github.io/)
	- [Pre-version of the course](http://karpathy.github.io/neuralnets/)
	- [Notes (Karpathy)](http://cs231n.github.io/)
	- [Videos for each lecture](https://www.youtube.com/playlist?list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC)
- #COURSE [Computer vision (NYU)](https://cs.nyu.edu/~fergus/teaching/vision/)
- #COURSE [Digital image processing (U Tartu)](https://sisu.ut.ee/dev/imageprocessing/avaleht)
- #COURSE Convolutional Neural Networks for Image Recognition (DeepMind x UCL | Deep Learning Lectures)
	- https://www.youtube.com/watch?v=shVKhOmT0HE&list=PLqYmG7hTraZCDxZ44o4p3N5Anz3lLRVZF&index=3&t=1s
	- https://storage.googleapis.com/deepmind-media/UCLxDeepMind_2020/L3%20-%20UUCLxDeepMind%20DL2020.pdf
- #COURSE Advanced Models for Computer Vision (DeepMind x UCL | Deep Learning Lectures)
	- https://www.youtube.com/watch?v=_aUq7lmMfxo&list=PLqYmG7hTraZCDxZ44o4p3N5Anz3lLRVZF&index=4
	- https://storage.googleapis.com/deepmind-media/UCLxDeepMind_2020/L4%20-%20UCLxDeepMind%20DL2020.pdf


## Code
- #CODE [Scikit-image. Image processing in Python](https://github.com/scikit-image/scikit-image)
	- http://scikit-image.org
- #CODE [OpenCV (Open Source Computer Vision Library)](https://opencv.org/)
	- OpenCV is released under a BSD license and hence it’s free for both academic and commercial use. It has C++, Python and Java interfaces and supports Windows, Linux, Mac OS, iOS and Android. OpenCV was designed for computational efficiency and with a strong focus on real-time applications. Written in optimized C/C++, the library can take advantage of multi-core processing. Enabled with OpenCL, it can take advantage of the hardware acceleration of the underlying heterogeneous compute platform.
	- https://github.com/opencv/opencv/wiki/Deep-Learning-in-OpenCV
	- #PAPER [Real-time computer vision with OpenCV (Pulli 2012)](https://dl.acm.org/doi/10.1145/2184319.2184337)
- #CODE [SimpleCV](https://github.com/sightmachine/SimpleCV)
	- http://simplecv.org/
	- SimpleCV is an open source framework for building computer vision applications. With it, you get access to several high-powered computer vision libraries such as OpenCV – without having to first learn about bit depths, file formats, color spaces, buffer management, eigenvalues, or matrix versus bitmap storage. This is computer vision made easy.
- #CODE [Imgaug. Image augmentation for machine learning experiments](https://github.com/aleju/imgaug)
	- http://imgaug.readthedocs.io
- #CODE [ChainerCV: a Library for Computer Vision in Deep Learning](https://github.com/chainer/chainercv)
		- http://chainercv.readthedocs.io/en/stable/
		- ChainerCV is a collection of tools to train and run neural networks for computer vision tasks using Chainer
- #CODE [Openface. Free and open source face recognition with deep neural networks](https://cmusatyalab.github.io/openface/)
- #CODE Vision - The torchvision package consists of popular datasets, model architectures, and common image transformations fo CV. 
	- https://github.com/pytorch/vision
- #CODE [Scenic](https://github.com/google-research/scenic)
	- https://www.marktechpost.com/2021/10/30/google-research-introduces-scenic-an-open-source-jax-library-for-computer-vision-research/
	- A Jax Library for Computer Vision Research and Beyond
	- codebase with a focus on research around attention-based models for computer vision


## References
### Deep learning-based CV
See: 
[CNNs](AI/Deep%20learning/CNNs.md)
[GANs](AI/Deep%20learning/GANs.md)
[Normalizing flows](AI/Deep%20learning/Normalizing%20flows.md)
[Transformers#For Computer Vision](AI/Deep%20learning/Transformers.md#For%20Computer%20Vision)

- [Deep Learning](AI/Deep%20learning/Deep%20Learning.md) is used in the domain of digital image processing to solve difficult problems (e.g.image colourization, classification, segmentation and  detection). DL methods such as [CNNs](AI/Deep%20learning/CNNs.md) mostly improve  prediction performance using big  data and plentiful computing resources and have pushed the boundaries of what was possible. Problems which were assumed to be unsolvable are now being solved with super-human accuracy. Image classification is a prime example of this. Since being reignited by Krizhevsky, Sutskever and Hinton in 2012, DL has dominated the domain ever since due to a substantially better performance compared to traditional methods.
- https://github.com/kjw0612/awesome-deep-vision
- https://github.com/timzhang642/3D-Machine-Learning
- https://medium.com/@taposhdr/medical-image-analysis-with-deep-learning-i-23d518abf531
- http://danielnouri.org/notes/2014/12/17/using-convolutional-neural-nets-to-detect-facial-keypoints-tutorial/

- #PAPER [Deep Learning for Computer Vision: A Brief Review (Voulodimos 2017)](https://www.hindawi.com/journals/cin/2018/7068349/)
- #PAPER [Deep Learning vs. Traditional Computer Vision (O'Mahony 2019)](https://arxiv.org/abs/1910.13796)
- #PAPER [Deep learning encodes robust discriminative neuroimaging representations to outperform standard machine learning (Abrol 2021)](https://www.nature.com/articles/s41467-020-20655-6)
- #PAPER [Deep learning-enabled medical computer vision (Esteva 2021)](https://www.nature.com/articles/s41746-020-00376-2)
- #PAPER [Involution: Inverting the Inherence of Convolution for Visual Recognition, a brand new neural operator (Li 2021)](https://arxiv.org/abs/2103.06255)
	- #CODE https://github.com/d-li14/involution
	- [Paper explained](https://www.youtube.com/watch?v=pH2jZun8MoY&list=WL&index=27&t=641s)
	- involution is a general-purpose neural primitive that is versatile for a spectrum of deep learning models on different vision tasks
	- involution bridges convolution and self-attention in design, while being more efficient and effective than convolution, simpler than self-attention in form
	- the proposed involution operator could be leveraged as fundamental bricks to build the new generation of neural networks for visual recognition, powering different deep learning models on several prevalent benchmarks
- #PAPER [Unifying Nonlocal Blocks for Neural Networks (Zhu 2021)](https://arxiv.org/abs/2108.02451v3)
	- #CODE https://github.com/zh460045050/SNL_ICCV2021


### Traditional CV techniques

#### Background subtraction
See [Background subtraction](AI/Computer%20Vision/Background%20subtraction.md)

#### Geometric transformations
- https://en.wikipedia.org/wiki/Geometric_transformation
- https://www.graphicsmill.com/docs/gm/affine-and-projective-transformations.htm
- https://docs.opencv.org/3.0-beta/doc/py_tutorials/py_imgproc/py_geometric_transformations/py_geometric_transformations.html
- http://eeweb.poly.edu/~yao/EL5123/lecture12_ImageWarping.pdf

##### Affine transformations 
- https://en.wikipedia.org/wiki/Affine_transformation
- Affine transformations are combinations of linear transformations and translations. Properties of affine transformations:
- Lines map to lines
- Parallel lines remain parallel
- Ratios are preserved
- Closed under composition

##### Projective transformations 
- https://en.wikipedia.org/wiki/Projective_transformation
- Projective transformations are combos of Affine transformations, and projective warps. Properties of projective transformations:
- Lines map to lines
- Parallel lines do not necessarily remain parallel
- Ratios are not preserved
- Closed under composition
- Models change of basis
- Projective matrix is defined up to a scale (8 DOF)


#### Filtering
- For each pixel we compute a function of local neighborhood and output a new value. Use cases:
- Enhance images: Denoise, smooth, increase contrast, etc.
- Extract information from images: Texture, edges, distinctive points, etc.
- Detect patterns: Template matching

https://dsp.stackexchange.com/questions/12684/difference-between-correlation-and-convolution-on-an-image

##### Spatial domain
- Linear filtering: function is a weighted sum/difference of pixel values (dot products at each position).
- [Convolution and kernels](https://en.wikipedia.org/wiki/Kernel_(image_processing))
- [Kernels visualization](http://setosa.io/ev/image-kernels/)
- http://scikit-image.org/docs/dev/api/skimage.filters.html
- Examples:
	- [Box filter. Replaces each pixel with an average of its neighborhood (smoothing effect)](https://en.wikipedia.org/wiki/Box_blur)
	- Sharpening filter. Accentuates differences with local average. 
		- http://northstar-www.dartmouth.edu/doc/idl/html_6.2/Sharpening_an_Image.html
		- https://en.wikipedia.org/wiki/Box_blur
	- Sobel filter. This filter is used in image processing and computer vision, particularly within edge detection algorithms where it creates an image emphasising edges. 
		- http://aishack.in/tutorials/sobel-laplacian-edge-detectors/
		- https://en.wikipedia.org/wiki/Sobel_operator
	- [Gaussian filter. Smoothing. Remove “high-frequency” components from the image (low-pass filter)](https://en.wikipedia.org/wiki/Gaussian_filter)
	- [Median filter. Non linear filter for image smoothing. Robustness to outliers](https://en.wikipedia.org/wiki/Median_filter)
	- [Bilateral filter. A bilateral filter is a non-linear, edge-preserving, and noise-reducing smoothing filter for images. It replaces the intensity of each pixel with a weighted average of intensity values from nearby pixels](https://en.wikipedia.org/wiki/Bilateral_filter)
	- Laplacian filter. Filtering with a Laplacian operator: 
		- http://aishack.in/tutorials/sobel-laplacian-edge-detectors/
		- https://docs.opencv.org/2.4/doc/tutorials/imgproc/imgtrans/laplace_operator/laplace_operator.html
		```
		  0		1		0
		  1 	-4		1
		  0 	1		0
		 ```
  
##### Frequency domain
- Fourier transform stores the magnitude and phase at each frequency. The magnitude encodes how much signal there is at a particular frequency whiel the phase encodes spatial information (indirectly). 
- The Convolution Theorem:
	- The Fourier transform of the convolution of two functions is the product of their Fourier transforms
	- The inverse Fourier transform of the product of two Fourier transforms is the convolution of the two inverse Fourier transforms
	- Convolutionin spatial domain is equivalent to multiplicationin frequency domain


#### Template matching
- https://en.wikipedia.org/wiki/Template_matching

##### Template based
- http://aishack.in/tutorials/template-matching/
- For templates without strong features, or for when the bulk of the template image constitutes the matching image, a template-based approach may be effective.
- Cross-correlation. Linear filtering: function is a weighted sum/difference of pixel values (dot products at each position)
	- https://en.wikipedia.org/wiki/Cross-correlation
	- [Convolution and kernels](https://en.wikipedia.org/wiki/Kernel_(image_processing))
	- [Kernels visualization](http://setosa.io/ev/image-kernels/)
- [Using image pyramids](https://en.wikipedia.org/wiki/Pyramid_(image_processing))


##### Feature based
- Feature-based approach relies on the extraction of image features such, i.e. shapes, textures , colors, to match in the target image or frame. This approach is currently achieved by using Neural Networks and Deep Learning classifiers such as VGG, AlexNet, ResNet. Deep Convolutional Neural Networks process the image by passing it through different hidden layers and at each layer produce a vector with classification information about the image. These vectors are extracted from the network and are used as the features of the image. Feature extraction by using Deep Neural Networks is extremely effective and thus is the standard in state of the art template matching algorithms.
- This method is considered more robust and is state of the art as it can match templates with non-rigid and out of plane transformation, it can match with high background clutter and illumination changes.

#### Feature extraction
The Computer Vision Pipeline, Part 4: feature extraction. https://freecontent.manning.com/the-computer-vision-pipeline-part-4-feature-extraction/
- Feature extraction is a core component of the computer vision pipeline. In fact, the entire deep learning model works around the idea of extracting useful features which clearly define the objects in the image. We’re going to spend a little more time here because it’s important that you understand what a feature is, what a vector of features is, and why we extract features.
- A feature in Machine Learning is an individual measurable property or characteristic of a phenomenon being observed. Features are the input that you feed to your machine learning model to output a prediction or classification. Suppose you want to predict the price of a house, your input features (properties) might include: square_foot, number_of_rooms, bathrooms, etc. and the model will output the predicted price based on the values of your features. Selecting good features that clearly distinguish your objects increases the predictive power of machine learning algorithms.

In image processing, algorithms are used to detect and isolate various desired portions or shapes (features) of a digitized image or video stream. It is particularly important in the area of optical character recognition. 
- Low-level: Edge detection, Corner detection, Blob detection, Ridge detection, Scale-invariant feature transform,
- Curvature: Edge direction, changing intensity, autocorrelation
- Image motion: Motion detection. Area based, differential approach, Optical flow (https://en.wikipedia.org/wiki/Optical_flow)
- Shape based: Thresholding, Blob extraction, Template matching, Hough transform
	- Lines: Circles/ellipses, Arbitrary shapes (generalized Hough transform). Works with any parameterizable feature (class variables, cluster detection, etc..)
- Flexible methods: Deformable, parameterized shapesActive contours (snakes)

##### Blob detection
- https://en.wikipedia.org/wiki/Blob_detection
- In computer vision, blob detection methods are aimed at detecting regions in a digital image that differ in properties, such as brightness or color, compared to surrounding regions. Informally, a blob is a region of an image in which some properties are constant or approximately constant; all the points in a blob can be considered in some sense to be similar to each other.
- [The Laplacian of Gaussian](https://en.wikipedia.org/wiki/Blob_detection#The_Laplacian_of_Gaussian)
- [The difference of Gaussians](https://en.wikipedia.org/wiki/Difference_of_Gaussians)
- [The determinant of the Hessian](https://en.wikipedia.org/wiki/Blob_detection#The_determinant_of_the_Hessian)
- [The hybrid Laplacian and determinant of the Hessian operator (Hessian-Laplace)](https://en.wikipedia.org/wiki/Blob_detection#The_hybrid_Laplacian_and_determinant_of_the_Hessian_operator_(Hessian-Laplace))
- [Maximally stable extremal regions (MSER)](https://en.wikipedia.org/wiki/Maximally_stable_extremal_regions)

##### Edge detection
- https://en.wikipedia.org/wiki/Template_matching
- [Canny edge detector](https://en.wikipedia.org/wiki/Canny_edge_detector)
	- The Canny edge detector is an edge detection operator that uses a multi-stage algorithm to detect a wide range of edges in images.
	- The Process of Canny edge detection algorithm can be broken down to 5 different steps:
		1. Apply Gaussian filter to smooth the image in order to remove the noise
		2. Find the intensity gradients of the image
		3. Apply non-maximum suppression to get rid of spurious response to edge detection
		4. Apply double threshold to determine potential edges
		5. Track edge by hysteresis: Finalize the detection of edges by suppressing all the other edges that are weak and not connected to strong edges.
	- http://aishack.in/tutorials/canny-edge-detector/
- Robert cross
	- https://en.wikipedia.org/wiki/Roberts_cross
	- The Roberts cross operator is used in image processing and computer vision for edge detection. 
	- As a differential operator, the idea behind the Roberts cross operator is to approximate the gradient of an image through discrete differentiation which is achieved by computing the sum of the squares of the differences between diagonally adjacent pixels.
- Prewitt operator
	- https://en.wikipedia.org/wiki/Prewitt_operator
	- The Prewitt operator is used in image processing, particularly within edge detection algorithms. Technically, it is a discrete differentiation operator, computing an approximation of the gradient of the image intensity function. At each point in the image, the result of the Prewitt operator is either the corresponding gradient vector or the norm of this vector. The Prewitt operator is based on convolving the image with a small, separable, and integer valued filter in horizontal and vertical directions and is therefore relatively inexpensive in terms of computations like Sobel and Kayyali operators. On the other hand, the gradient approximation which it produces is relatively crude, in particular for high frequency variations in the image.
- Deriche edge detector
	- https://en.wikipedia.org/wiki/Deriche_edge_detector
	- The Prewitt operator is used in image processing, particularly within edge detection algorithms. Technically, it is a discrete differentiation operator, computing an approximation of the gradient of the image intensity function. At each point in the image, the result of the Prewitt operator is either the corresponding gradient vector or the norm of this vector. The Prewitt operator is based on convolving the image with a small, separable, and integer valued filter in horizontal and vertical directions and is therefore relatively inexpensive in terms of computations like Sobel and Kayyali operators. On the other hand, the gradient approximation which it produces is relatively crude, in particular for high frequency variations in the image.

##### Corner detection
- https://en.wikipedia.org/wiki/Corner_detection
- http://aishack.in/tutorials/corner-detection-opencv/
- Corner detection is an approach used within computer vision systems to extract certain kinds of features and infer the contents of an image.
- [Harris operator: detects corners (patches that have strong gradients in two orthogonal directions)](https://en.wikipedia.org/wiki/Harris_Corner_Detector)
- [Förstner corner detector](https://en.wikipedia.org/wiki/Corner_detection#The_F%C3%B6rstner_corner_detector)
- [The Wang and Brady corner detection algorithm](https://en.wikipedia.org/wiki/Corner_detection#The_Wang_and_Brady_corner_detection_algorithm)
- [The SUSAN corner detector](https://en.wikipedia.org/wiki/Corner_detection#The_SUSAN_corner_detector)
- [The Trajkovic and Hedley corner detector](https://en.wikipedia.org/wiki/Corner_detection#The_Trajkovic_and_Hedley_corner_detector)

##### Feature descriptors
- Scale-invariant feature transform (SIFT)
	- http://aishack.in/tutorials/sift-scale-invariant-feature-transform-introduction/
	- SIFT keypoints of objects are first extracted from a set of reference images and stored in a database. An object is recognized in a new image by individually comparing each feature from the new image to this database and finding candidate matching features based on Euclidean distance of their feature vectors. From the full set of matches, subsets of keypoints that agree on the object and its location, scale, and orientation in the new image are identified to filter out good matches. The determination of consistent clusters is performed rapidly by using an efficient hash table implementation of the generalised Hough transform. Each cluster of 3 or more features that agree on an object and its pose is then subject to further detailed model verification and subsequently outliers are discarded. Finally the probability that a particular set of features indicates the presence of an object is computed, given the accuracy of fit and number of probable false matches. Object matches that pass all these tests can be identified as correct with high confidence.
	- https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_sift_intro/py_sift_intro.html
	- There are mainly five steps involved in SIFT algorithm.
		1. Scale-space Extrema Detection (using DoG)
		2. Keypoint Localization
		3. Orientation Assignment
		4. Keypoint Descriptor
		5. Keypoint Matching
- [Histogram of oriented gradients (HOG)](https://en.wikipedia.org/wiki/Histogram_of_oriented_gradients)
- Speeded up robust features (SURF)
	- https://en.wikipedia.org/wiki/Speeded_up_robust_features
	- In computer vision, speeded up robust features (SURF) is a patented local feature detector and descriptor. It can be used for tasks such as object recognition, image registration, classification or 3D reconstruction. It is partly inspired by the scale-invariant feature transform (SIFT) descriptor. The standard version of SURF is several times faster than SIFT and claimed by its authors to be more robust against different image transformations than SIFT.

##### Kanade–Lucas–Tomasi (KLT) feature tracker
- https://en.wikipedia.org/wiki/Kanade%E2%80%93Lucas%E2%80%93Tomasi_feature_tracker
- In computer vision, the Kanade–Lucas–Tomasi (KLT) feature tracker is an approach to feature extraction. It is proposed mainly for the purpose of dealing with the problem that traditional image registration techniques are generally costly. KLT makes use of spatial intensity information to direct the search for the position that yields the best match. It is faster than traditional techniques for examining far fewer potential matches between the images.
- Summary of KLT tracking:
	- Find a good point to track (harriscorner)
	- Use intensity second moment matrix and difference across frames to find displacement
	- Iterate and use coarse-to-fine search to deal with larger movements 
	- When creating long tracks, check appearance of registered patch against appearance of initial patch to find points that have drifted

##### Optical flow
- https://en.wikipedia.org/wiki/Optical_flow
- Vector field function of the spatio-temporal image brightness variations 
- #PAPER [Large Displacement Optical Flow](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/papers/brox_cvpr09.pdf)


