---
title: "Individual tree segmentation with lidar"
excerpt: "This project experiments with using the SegmentAnyTree deep learning model on lidar data from the Amazon rainforest. <br/><img src='/images/segment-trees.png'>"
collection: portfolio
---

Segmentation of individual trees from lidar allows for fine-grained forest carbon calculations. The recent paper SegmentAnyTree developed a deep learning model that used a data augmentation approach to allow the model to be sensor and platform agnostic. I decided to try out the model on some airborne lidar (ALS) data from Paisagens Sustentáveis scans of the Amazon in Brazil. As pointed out in the paper, the SegmentAnyTree model was trained primarily on coniferous managed forests and performs best in those environments, but I was interested to give it a try on a very different type of forest and see the result. From this project I learned about the characteristics of different lidar platforms, processing and visualizing lidar data, 3D CNNs for segmenting voxelized point clouds, and building docker images using Google Cloud Build.

As expected, the results were mixed as you can see in this sample of 20 segmented instances.

![segmentation results](/images/segment-trees.png)

Improved results could be achieved by further training the model on high quality labeled data from this region.

SegmentAnyTree [paper](https://www.sciencedirect.com/science/article/pii/S0034425724003936) and [Github repository](https://github.com/SmartForest-no/SegmentAnyTree)