# Custom VGG16 Model for Tiny ImageNet Classification
## Abstract
The dataset for this project is a small scale version of the ImageNet Large Scale Visual Recognition Challenge (ILSVRC). In this project, I approached the image classification problem by using transfer learning on custom VGG16 CNN architecture. I have also applied data augmentation methods to training images, hoping to artificially create variations that help the model to generalize better. Considering the small size of the dataset, the model performed well.
## Dataset
The dataset contains square images, of 64×64 pixels. Most of the images have 3 channels for color, RGB, meaning they are 64x64x3 arrays. However, some of the examples are grayscale images, i.e. 64×64×1 arrays. For the sake of simplicity, all the grayscale images are immediately converted to RGB by replicating the pixel values across the three channels. Each image belongs to exactly one out of 200 categories. The training set contains 90,000 images (450 from each category), and the validation and test sets have 10,000 images each (50 from each category).
The dataset can be downloaded from <a href="https://drive.google.com/file/d/116KlGk5ExxS5QCaIQBXRxWCC4SzNjYVB/view?usp=sharing">here.</a>
## Getting Started
The `custom_vgg16_for_tiny_imagenet.ipynb` notebook can be directly run on Kaggle after loading the dataset in the Kaggle Kernel. Use Kaggle's Nvidia Tesla P100 GPU for faster training and evaluation.

### Pre-Requisites
For running the notebook on your local machine, following pre-requisites must be satisfied:
- Python3
- NumPy
- Pandas
- Matplotlib
- Tensorflow 2.X
- Keras
### Installing
After ensuring you have the above mentioned versions of Tensorflow and Python. The other two prerequisites can be installed in the notebook as:

Keract:
```Python
!pip install keract
```
Keras-Contrib:
```
!pip install git+https://github.com/keras-team/keras-contrib.git
```
## Detailed Report
A detailed report of this project is available <a href="https://drive.google.com/file/d/1teDoAIaFQiQ5u_-ULcGo4QIi9Qxezqui/view?usp=sharing">here.</a>
## Authors
* Ayush Dabra
## Acknowledgements
I express my sincere thanks to Dr. Laxmidhar Behera, who provided me with the opportunity to work on this project. I pay my deep sense of gratitude to Dr. Vipul Arora, without his valuable guidance and supervision the project couldn't have been completed.
## Third Party Libraries
- Keract by Philippe Rémy (@github/philipperemy) used under the IT License Copyright (c) 2019.
- Keras-Contrib by Keras (@github.com/keras-team), now deprecated and managed by Keras Community Contributors, used under MIT License Copyright (c) 2017 Fariz Rahman.
