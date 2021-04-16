# Face-Mask-Detector
![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Django.svg)

Creating a Face mask detctor using CNN on Tensorflow keras
## :star: TechStack/framework used

- [OpenCV](https://opencv.org/)
- [Caffe-based face detector](https://caffe.berkeleyvision.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)
- 
## :file_folder: Dataset
The dataset used can be downloaded here - [Click to Download](https://drive.google.com/file/d/1L_3kDRWL24iecb4IvxvjF_npdmzWzSWW)

This dataset consists of __4095 images__ belonging to two classes:
*	__with_mask: 2165 images__
*	__without_mask: 1930 images__

The images used were real images of faces wearing masks. The images were collected from the following sources:

* __Bing Search API__ ([See Python script](https://github.com/ombhatia99/Face-Mask-Detector/blob/main/search.py))
* __Kaggle datasets__ 
* __RMFD dataset__ ([See here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset))([medium article link](https://medium.com/the-programming-hub/wolrds-most-complete-masked-face-recognition-dataset-is-for-free-10d780eed512))

## :key: Prerequisites

All the dependencies and required libraries are included in the file <code>requirements.txt</code> 
## Result
Hyperparameter: 
    - batch size: 32
    - Learing rate: 0.0001
    - Input size: 64x64x3

The Pre-trained models used can be downloaded here - [Click to Download](https://drive.google.com/file/d/1IzX6C0Sn-SJyFOdfFCrylvAbe8XnRdi8)

Model result
| Model         | Test Accuracy| Size        | Params    | Memory consumption|
| ------------- | -------------|-------------|-----------|-------------------|
| CNN           |  87.67%      | 27.1MB      | 2,203,557 | 72.58 MB
| VGG16         |  93.08%      | 62.4MB      | **288,357**    | **18.06 MB**
| MobileNetV2 (fine tune)  |  97.33%      | **20.8MB**  | 1,094,373 | 226.67 MB
| **Xception**  | **98.33%**   | 96.6MB      | 1,074,789 | 368.18 MB

