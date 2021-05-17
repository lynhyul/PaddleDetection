# PaddleDetection

English | 简体中文

PaddleDetection 2.0 is ready! Dygraph mode is set by default and static graph code base is here
Highly effective PPYOLO v2 and ultra lightweight PPYOLO tiny are released! link
SOTA Anchor Free model -- PAFNet is released! link
Recent Activity
A series of live lectures on detailed explanation of industrial-level object detection technology is about to be launched，to see how powerful PP-YOLOv2 surpasses YOLOv5.

Welcome to the PPYLOv2 &Tiny Tech Seminar Group


Course Schedule
Live Link

May 13rd 19:00-20:00
Topic: Detailed Interpretation of Industrial-level Object Detection Algorithms
May 14th 19:00-20:00
Topic: Analysis and Application of 1.3M Ultra-lightweight Object Detection Algorithm
May 21st 20:00-21:00
Topic: The Model Development Exercise of Small Target Detection Under Complex Background
Course Link
0【PaddleDetection2.0 Special】Quick Experience of New Version

1【PaddleDetection2.0 Special】How to Customize Dataset

2【PaddleDetection2.0 Special】Quick Start PP-YOLOv2

3【PaddleDetection2.0 Special】Quick Start PP-YOLO tiny

4【PaddleDetection2.0 Special】Quick Start S2ANet

5【PaddleDetection2.0 Special】Fast Implementation of Pedestrian Detection

6【PaddleDetection2.0 Special】Fast Implementation of Face Detection

Introduction
PaddleDetection is an end-to-end object detection development kit based on PaddlePaddle, which aims to help developers in the whole development of constructing, training, optimizing and deploying detection models in a faster and better way.

PaddleDetection implements varied mainstream object detection algorithms in modular design, and provides wealthy data augmentation methods, network components(such as backbones), loss functions, etc., and integrates abilities of model compression and cross-platform high-performance deployment.

After a long time of industry practice polishing, PaddleDetection has had smooth and excellent user experience, it has been widely used by developers in more than ten industries such as industrial quality inspection, remote sensing image object detection, automatic inspection, new retail, Internet, and scientific research.


Product news
2021.04.14: Release release/2.0 version. Dygraph mode in PaddleDetection is fully supported. Cover all the algorithm of static graph and update the performance of mainstream detection models. Release PP-YOLO v2 and PP-YOLO tiny, enhanced anchor free model PAFNet and S2ANet which is aimed at rotation object detection.Please refer to PaddleDetection for details.
2020.02.07: Release release/2.0-rc version, Please refer to PaddleDetection for details.
Features
Rich Models PaddleDetection provides rich of models, including 100+ pre-trained models such as object detection, instance segmentation, face detection etc. It covers a variety of global competition champion schemes.

Highly Flexible: Components are designed to be modular. Model architectures, as well as data preprocess pipelines and optimization strategies, can be easily customized with simple configuration changes.

Production Ready: From data augmentation, constructing models, training, compression, depolyment, get through end to end, and complete support for multi-architecture, multi-device deployment for cloud and edge device.

High Performance: Based on the high performance core of PaddlePaddle, advantages of training speed and memory occupation are obvious. FP16 training and multi-machine training are supported as well.

Overview of Kit Structures
Architectures	Backbones	Components	Data Augmentation
Two-Stage Detection
Faster RCNN
FPN
Cascade-RCNN
Libra RCNN
Hybrid Task RCNN
PSS-Det RCNN
One-Stage Detection
RetinaNet
YOLOv3
YOLOv4
PP-YOLO
SSD
Anchor Free
CornerNet-Squeeze
FCOS
TTFNet
Instance Segmentation
Mask RCNN
SOLOv2
Face-Detction
FaceBoxes
BlazeFace
BlazeFace-NAS
ResNet(&vd)
ResNeXt(&vd)
SENet
Res2Net
HRNet
Hourglass
CBNet
GCNet
DarkNet
CSPDarkNet
VGG
MobileNetv1/v3
GhostNet
Efficientnet
Common
Sync-BN
Group Norm
DCNv2
Non-local
FPN
BiFPN
BFP
HRFPN
ACFPN
Loss
Smooth-L1
GIoU/DIoU/CIoU
IoUAware
Post-processing
SoftNMS
MatrixNMS
Speed
FP16 training
Multi-machine training
Resize
Flipping
Expand
Crop
Color Distort
Random Erasing
Mixup
Cutmix
Grid Mask
Auto Augment
Overview of Model Performance
The relationship between COCO mAP and FPS on Tesla V100 of representative models of each architectures and backbones.


NOTE:

CBResNet stands for Cascade-Faster-RCNN-CBResNet200vd-FPN, which has highest mAP on COCO as 53.3%

Cascade-Faster-RCNN stands for Cascade-Faster-RCNN-ResNet50vd-DCN, which has been optimized to 20 FPS inference speed when COCO mAP as 47.8% in PaddleDetection models

PP-YOLO achieves mAP of 45.9% on COCO and 72.9FPS on Tesla V100. Both precision and speed surpass YOLOv4

PP-YOLO v2 is optimized version of PP-YOLO which has mAP of 49.5% and 68.9FPS on Tesla V100

All these models can be get in Model Zoo

Tutorials
Get Started
Installation guide
Quick start on small dataset
Prepare dataset
Train/Evaluation/Inference/Deploy
Advanced Tutorials
Parameter configuration

Parameter configuration for RCNN model
Parameter configuration for PP-YOLO model
Model Compression(Based on PaddleSlim)

Prune/Quant/Distill
Inference and deployment

Export model for inference
Python inference
C++ inference
Serving
Inference benchmark
Advanced development

New data augmentations
New detection algorithms
Model Zoo
Universal object detection
Model library and baselines
PP-YOLO
Enhanced Anchor Free model--TTFNet
Mobile models
676 classes of object detection
Two-stage practical PSS-Det
SSLD pretrained models
Universal instance segmentation
SOLOv2
Rotation object detection
S2ANet
Vertical field
Face detection
Pedestrian detection
Vehicle detection
Competition Plan
Objects365 2019 Challenge champion model
Best single model of Open Images 2019-Object Detction
Applications
Christmas portrait automatic generation tool
Updates
v2.0 was released at 04/2021, fully support dygraph version, which add BlazeFace, PSS-Det and plenty backbones, release PP-YOLOv2, PP-YOLO tiny and S2ANet, support model distillation and VisualDL, add inference benchmark, etc. Please refer to change log for details.

License
PaddleDetection is released under the Apache 2.0 license.

Contributing
Contributions are highly welcomed and we would really appreciate your feedback!!

Citation
@misc{ppdet2019,
title={PaddleDetection, Object detection and instance segmentation toolkit based on PaddlePaddle.},
author={PaddlePaddle Authors},
howpublished = {\url{https://github.com/PaddlePaddle/PaddleDetection}},
year={2019}
}
