---
title: "Object detection"
---

> See [[AI/Computer Vision/Semantic segmentation]]
 
## Code
- https://github.com/microsoft/computervision-recipes/tree/master/scenarios/detection
- #CODE [MMdetection](https://github.com/open-mmlab/mmdetection)
	- OpenMMLab Detection Toolbox and Benchmark (pytorch)
	- https://mmdetection.readthedocs.io/
- #CODE TensorFlow object detection API
	- [Repository](https://github.com/tensorflow/models/tree/master/research/object_detection)
	- [Model zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md)
	- https://medium.com/swlh/train-your-custom-object-detector-with-tensorflow-object-detector-api-65d38dcdf08c
	- https://modelzoo.co/model/objectdetection
- #CODE [Detectron2](https://github.com/facebookresearch/detectron2)
	- Detectron2 is FAIR's next-generation platform for object detection and segmentation
- #CODE https://github.com/jinwchoi/awesome-action-recognition#object-detection
- #CODE [YOLO: Real-Time Object Detection](https://pjreddie.com/darknet/yolo/)

## References
Review papers:
- #PAPER [Recent Advances in Object Detection in the Age of Deep [CNNs](AI/Deep%20learning/CNNs.md) (Agarwal 2019)](https://arxiv.org/abs/1809.03193)
- #PAPER [Deep learning for Generic Object Detection: A Survey (Liu 2019)](https://arxiv.org/abs/1809.02165v4)


- #PAPER [Multiple Object Recognition with Visual Attention (Ba 2015)](http://arxiv.org/abs/1412.7755)
- #PAPER Is object localization for free? – Weakly Supervised Object Recognition with Convolutional Neural Networks (Oquab 2015): 
	- http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Oquab_Is_Object_Localization_2015_CVPR_paper.pdf
	- https://www.di.ens.fr/willow/research/weakcnn/
- #PAPER [DeepLab - Weakly-and semi-supervised learning of a DCNN for semantic image segmentation (Papandreou 2015)](http://arxiv.org/abs/1502.02734)
- #PAPER [SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation (Badrinarayanan 2016)](http://arxiv.org/abs/1511.00561)
- #PAPER [SSD. Single Shot MultiBox Detector (Liu 2016)](https://arxiv.org/abs/1512.02325)
	- #BOOK https://d2l.ai/chapter_computer-vision/ssd.html
- #PAPER [YOLO. You Only Look Once: Unified, Real-Time Object Detection (Redmon 2016)](https://arxiv.org/abs/1506.02640)
	- YOLO or You Only Look Once is an object detection algorithm much different from the region based algorithms. In YOLO a single convolutional network predicts the bounding boxes and the class probabilities for these boxes.
	- How YOLO works is that we take an image and split it into an SxS grid, within each of the grid we take m bounding boxes. For each of the bounding box, the network outputs a class probability and offset values for the bounding box. The bounding boxes having the class probability above a threshold value is selected and used to locate the object within the image.
- #PAPER [RetinaNet. Focal Loss for Dense Object Detection (Lin 2018)](https://arxiv.org/abs/1708.02002)
	- #CODE https://github.com/fizyr/keras-retinanet
	- https://keras.io/examples/vision/retinanet/
	- https://towardsdatascience.com/object-detection-on-aerial-imagery-using-retinanet-626130ba2203
- #PAPER [CornerNet: Detecting Objects as Paired Keypoints (Law 2018)](https://arxiv.org/abs/1808.01244)
	- #CODE https://github.com/makalo/CornerNet
- #PAPER [ExtremeNet. Bottom-up Object Detection by Grouping Extreme and Center Points (Zhou 2019)](https://arxiv.org/abs/1901.08043)
	- #CODE https://github.com/xingyizhou/ExtremeNet
- #PAPER [EfficientDet: Scalable and Efficient Object Detection (Tan 2020)](https://arxiv.org/pdf/1911.09070.pdf)
	- #CODE https://github.com/xuannianz/EfficientDet
	- Included in the TF object detection API
- #CODE [YOLOX: Exceeding YOLO Series in 2021 (Ge 2021)](https://arxiv.org/abs/2107.08430v1)
	- #CODE https://paperswithcode.com/paper/yolox-exceeding-yolo-series-in-2021

Region-based CNNs (R-CNNs):
- https://www.pyimagesearch.com/2020/07/06/region-proposal-object-detection-with-opencv-keras-and-tensorflow/
- #BOOK [Region-based RCNNs](https://d2l.ai/chapter_computer-vision/rcnn.html)
- #PAPER [Regional CNN (R-CNN)](https://arxiv.org/abs/1311.2524)
	- The goal of R-CNN is to take in an image, and correctly identify where the main objects (via a bounding box) in the image.
	- R-CNN creates these bounding boxes, or region proposals, using a process called Selective Search. 
	- Once the proposals are created, R-CNN warps the region to a standard square size and passes it through to a modified version of AlexNet (the winning submission to ImageNet 2012 that inspired R-CNN).
	- On the final layer of the CNN, R-CNN adds a Support Vector Machine (SVM) that simply classifies whether this is an object, and if so what object. 
- #PAPER [Fast R-CNN](https://arxiv.org/abs/1504.08083)
	- RoI (Region of Interest) Pooling. At its core, RoIPool shares the forward pass of a CNN for an image across its subregions. 
	- The second insight of Fast R-CNN is to jointly train the CNN, classifier, and bounding box regressor in a single model. 
- #PAPER [Faster R-CNN](https://arxiv.org/abs/1506.01497)
	- The insight of Faster R-CNN was that region proposals depended on features of the image that were already calculated with the forward pass of the CNN (first step of classification).
	- So why not reuse those same CNN results for region proposals instead of running a separate selective search algorithm?
	- A single CNN is used to both carry out region proposals and classification. This way, only one CNN needs to be trained and we get region proposals almost for free. Faster R-CNN adds a Fully Convolutional Network on top of the features of the CNN creating what’s known as the Region Proposal Network.
- #PAPER [Mask R-CNN (He 2018)](https://arxiv.org/abs/1703.06870)
	- Extending Faster R-CNN for Pixel Level Segmentation
	- Mask R-CNN does this by adding a branch to Faster R-CNN that outputs a binary mask that says whether or not a given pixel is part of an object. The branch, as before, is just a Fully Convolutional Network on top of a CNN based feature map. 
	- But the Mask R-CNN authors had to make one small adjustment to make this pipeline work as expected: Realigning RoIPool to be More Accurate.
	- https://engineering.matterport.com/splash-of-color-instance-segmentation-with-mask-r-cnn-and-tensorflow-7c761e238b46
	- https://modelzoo.co/model/mask-r-cnn-keras
	- https://machinelearningmastery.com/how-to-train-an-object-detection-model-with-keras/