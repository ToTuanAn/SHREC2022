# SHREC 2022: Fitting and recognition of simple geometric primitives on point clouds

![header](img/models.png)
The aim of this SHREC track is to evaluate the quality of automatic algorithms for fitting and recognising geometric primitives in point clouds. The goal is to identify, for each point cloud, its primitive type and some geometric descriptors. As simple primitives we mean the classical surface primitives derived from constructive solid geometry, i.e., planes, spheres, cylinders, cones and tori. We admit that some point clouds might be unfitted by one of these simple primitives.

## Table of Content

### [Dataset](#dataset)
### [Data preprocessing](#preprocessing)
### [Trainning](#training)
### [Evaluation](#evaluatation)

## Data preprocessing
Given the raw data, we need to upscale the pointclouds data to a constant value. To do that, we can run the following code
```sh
python preprocessing.py
```
We provided a code to change .txt file to .ply if needed
```sh
python txt2ply.py
```

## Training
For training, we employed pointNet architecture. Pretrained models are save in the model/ directory. 
```sh
python train.py 
``` 

## Evaluation 
```sh
python eval.py 
``` 



