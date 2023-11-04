---
title: You Only Learn Yolov8 in One
date: 2023-11-04 10:07:40
updated: 2023-11-04 10:07:40
tags: Yolov8
categories:
- DeepLearning
- ObjectDetection
cover: https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcReC2WEKvgGPCIbrMPf9OC7y6odxYyDKo9drPtpkmhCmZ5KGtR4BWmROLF9oN-ocBXX_g&usqp=CAU
---

## Start and Try

```bash
# Install the ultralytics package from PyPI
pip install ultralytics
# predict and youtube vedio and execute segment
yolo predict model=yolov8n-seg.pt source='https://youtu.be/LNwODJXcvt4' imgsz=320
# some special command
yolo help
yolo checks
yolo version
yolo settings
yolo copy-cfg
yolo cfg

```
<!-- more -->


## Modes

### Train

#### start Train

Training a deep learning model involves feeding it data and adjusting its parameters so that it can make accurate predictions. 

If no argument is passed GPU `device=0` will be used if available, otherwise `device=cpu` will be used. See Arguments section below for a full list of training arguments.

Example:

```python
from ultralytics import YOLO

# Load a model
model = YOLO('yolov8n.yaml')  # build a new model from YAML
model = YOLO('yolov8n.pt')  # load a pretrained model (recommended for training)
model = YOLO('yolov8n.yaml').load('yolov8n.pt')  # build from YAML and transfer weights

# Train the model
results = model.train(data='coco128.yaml', epochs=100, imgsz=640)

```

#### Resume Paused Task

```python
from ultralytics import YOLO

# Load a model
model = YOLO('path/to/last.pt')  # load a partially trained model

# Resume training
results = model.train(resume=True)

```

#### Parameters That Can Be Introduced in Common

| key      | Value(default) | Description                          |
| -------- | -------------- | ------------------------------------ |
| model    | None           | path to model, yolov8n.pt            |
| data     | None           | Path to data file, coco128.yaml      |
| epoch    | 100            | number of epoch                      |
| patience | 50             | using in early stop method           |
| batch    | 16             | images per batch                     |
| imgsz    | 640            | size of input images                 |
| save     | True           | save checkpoint or results           |
| device   | None           | device to run                        |
| project  | None           | project name                         |
| name     | None           | experiment name                      |
| seed     | 0              | random seed for reproducibility      |
| resume   | False          | resume training from last checkpoint |

There are some extra parameters about device performances or train process, refer to original web page. I only list some that I use frequent in reality here.



### Validation

#### Example

```python
from ultralytics import YOLO

# Load a model
model = YOLO('yolov8n.pt')  # load an official model
# model = YOLO('path/to/best.pt')  # load a custom model

# Validate the model
metrics = model.val()  # no arguments needed, dataset and settings remembered
metrics.box.map    # map50-95
metrics.box.map50  # map50
metrics.box.map75  # map75
metrics.box.maps   # a list contains map50-95 of each category

```

#### Settings in Common

Hyperparameters and configurations affect model’s performance, speed and accuracy.

Note for two things: Performance and overfitting.

| key         | Val(default) | Description                               |
| ----------- | ------------ | ----------------------------------------- |
| data        | None         | path to data                              |
| imgsz       | 640          | size of input                             |
| batch       | 16           | number of per batch                       |
| save_json   | False        | save result to json                       |
| save_hybrid | False        | save hybrid of lables                     |
| conf        | 0.001        | object confidence threshold for detection |
| iou         | 0.6          | intersection over union threshold for NMS |
| device      | None         | device                                    |
| plots       | False        | show plats during training                |
| split       | val          | dataset split to use for validation       |