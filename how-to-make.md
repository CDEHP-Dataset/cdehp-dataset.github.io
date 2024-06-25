---
layout: default
title: How to Make CDEHP-Dataset
permalink: /how-to-make
---

## Introduction

We fixed a depth camera and an event camera on a simple tripod, and took action videos from a number of volunteers. The data annotations are obtained by using crowdsourcing with post-reviewing.


## Hardware Requirement

* A depth camera (We used `Intel® RealSense™ D435i`).
* An event-based camera/dynamic vision sensor (We used `CelePixel CeleX5`).
* An infrared filter, which was to filter out the infrared spectrum from the depth camera to protect the event camera from the spectrum interference.

## Building the Camera Stand

We strongly recommend to use a 3D printing technology to make a simple fixture to hold two or more cameras, avoiding the vibration after the calibration.

![Cameras Stand](/assets/how-to-make_1.png)

## Camera calibration

We employed `Zhang's method` for the stereo camera calibration to obtain the parameters between the two cameras. After that, we used the homography transformation algorithm to convert the annotations of key points on the RGB images to the locations on the corresponding event frames.

1. Prepare a `Calibration Patterns Board(Checkerboards)`. A bigger board can get the better accuracy, since it can accurately calculate longer-distance movements.
2. Use [Shooting Tool](https://github.com/CDEHP-Dataset/Tools/tree/main/calibration) to capture a number of images at different angles, distances and locations.
3. Detect key points of the chessboard on all captured images. We used `Camera Calibrator` App in `MATLAB`.
4. Use [Calibration-Tool](https://github.com/CDEHP-Dataset/Calibration-Tool) calculate parameters between cameras.

## Recording Dataset

Use [Recording-Tool](https://github.com/CDEHP-Dataset/Recording-Tool) to record dataset.

## Label Dataset

Use [Annotation-Tool](https://github.com/CDEHP-Dataset/Annotation-Tool) to label the dataset.
