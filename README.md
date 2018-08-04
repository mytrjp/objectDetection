 
#### Object Detection by Tensorflow Object Detection API 
 - Workshop Tutorial
 - August 2, 2018
 
![alt text](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/img/kites_detections_output.jpg "kites")

---

- About the Repo
   * API     : Tensorflow's Object Detection API
   * ckpt    : trained model parameters saved
   * config  : Configuration settings
   * eval    : Evaluation result folder
   * figures : helper figures for understanding Faster-RCNN
   * frozen_model : Inference graph of trained model
   * images : 
      * train/val/test data
      * converted csv files
      * converted tfrecord files
      * labelmap.pbtxt : defines labels
   * pretrained   : Pretrained model parameters 

---
 
## 1. Introduction

### 1.1. Datasets
--> [Datasets](https://www.analyticsvidhya.com/blog/2018/03/comprehensive-collection-deep-learning-datasets/)
- COCO
- KITTI
- Pascal
- Oid
- AVA v2.1 trained models
- Open Images-trained models

### 1.2. Landmark Papers

>> 2-Stage Detectors
 - [Mask-RCNN](https://arxiv.org/pdf/1703.06870)
 - [Faster-RCNN](https://arxiv.org/pdf/1506.01497)
 - [Fast-RCNN](https://arxiv.org/pdf/1504.08083)
 - [RCNN](https://arxiv.org/pdf/1311.2524)
 - [Selective Search](http://www.huppelen.nl/publications/selectiveSearchDraft.pdf)
 
>> 1-Stage Detectors
 - [YOLO](https://arxiv.org/pdf/1506.02640)
 - [SSD](https://arxiv.org/abs/1512.02325)
 - [OverFeat](https://arxiv.org/abs/1312.6229)

>> Review
 - [Speed/Accuracy Trade-off](https://arxiv.org/abs/1611.10012)


### 1.3. Feature Extractors

- VGG
- ZFNet
- MobileNet
- Inception
- ResNet
- DenseNet

## 2. Prepare Input Pipeline

### 2.1.Download Images

- Google Advanced Image Search
 * birds , tigers , rabbits etc..
 
- Downloader Tools (Chrome Extensions):
 * Download All Images 2.0.4
 * Fatkun Batch Download Image 2.23


### 2.2. Annotate Objects

- Bounding Box
 * [LabelImg](https://github.com/tzutalin/labelImg)
- Polygon
- Semantic Segmentation
- Bounding Box
- Line

### 2.3. Data Format Conversion

- xml_to_csv
- csv_to_tfrecord
- resizer
- extension check
- size check

### 2.4. API Introduction

 - [Download API](https://github.com/tensorflow/models/tree/master/research/object_detection)
 - [configuration files](https://github.com/tensorflow/models/tree/master/research/object_detection/samples/configs)
 - [configuration settings](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/configuring_jobs.md)
 - [models/research/object_detection/g3doc/detection_model_zoo.md](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md)

## 3. Set Colab Environment

 - Install Requirements
 - Connect Drive
 - Clone Repository
 - Set python environment
 - train
 - ..


## 4. Useful Links (References)
- [Protobuf](https://towardsdatascience.com/3-steps-to-update-parameters-of-faster-r-cnn-ssd-models-in-tensorflow-object-detection-api-7eddb11273ed)
- [Annotation](https://blog.playment.io/comparing-image-annotation-types/)

- [Tryo Labs Object Detection Tutorial](https://tryolabs.com/blog/2018/01/18/faster-r-cnn-down-the-rabbit-hole-of-modern-object-detection/)
-[Edge Electronics Tutorial](https://github.com/EdjeElectronics/TensorFlow-Object-Detection-API-Tutorial-Train-Multiple-Objects-Windows-10)
- [Speed/accuracy trade-off by Jonathan Hui](https://medium.com/@jonathan_hui/object-detection-speed-and-accuracy-comparison-faster-r-cnn-r-fcn-ssd-and-yolo-5425656ae359)
- [Tensorflow Object Detection on Google Colab](https://medium.com/@moshe.livne/training-tensorflow-for-free-pet-object-detection-api-sample-trained-on-google-collab-c2e65f4a9949)

