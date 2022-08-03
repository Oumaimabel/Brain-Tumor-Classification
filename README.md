# A Deep Learning Approach for Brain Tumor Detection and Classification

### Introduction
Automatic segmentation and classification of medical images play an important role in diagnostics, growth prediction, and treatment of brain tumors. An early tumor brain diagnosis implies a faster response in treatment, which helps to improve patients’ survival rate. Location and classification of brain tumors in large medical images databases, taken in routine clinical tasks by manual procedures, have a high cost both in effort and time. An automatic detection, location, and classification procedure is desirable and worthwhile.

### About Dataset
This brain tumor dataset containing 3064 T1-weighted contrast-enhanced MRI (T1w CE-MRI) images from 233 patients with three kinds of brain tumor:

![4](https://user-images.githubusercontent.com/93741954/182624390-27564850-e9c3-49bd-8e56-eabe255857a2.png)
![5](https://user-images.githubusercontent.com/93741954/182624472-f40935ee-24b0-4c67-9dfa-31293048114f.png)
![2](https://user-images.githubusercontent.com/93741954/182621291-d0523a53-88c3-4a70-9ce4-8ae76ed85c7c.png)

The dataset was used in the following research papers:
- Cheng, Jun, et al. "Enhanced Performance of Brain Tumor Classification via Tumor Region Augmentation and Partition." PloS one 10.10 (2015).
- Cheng, Jun, et al. "Retrieval of Brain Tumors by Adaptive Spatial Pooling and Fisher Vector Representation." PloS one 11.6 (2016).

### How to run
Before executing the Google Colab notebook make sure you can access the dataset from your Google Colab notebook for which you can create the shortcut to the Google Drive link: https://drive.google.com/drive/folders/1BrPSLL6AxZortFKJW3aqCBQztXBdD8Qp?usp=sharing on your google drive and then set the path to this shortcut by changing the value of DATA_PATH_DIR variable in the notebook to get access to the datasets after you have given access to your google drive by executing the following piece of code:
![1](https://user-images.githubusercontent.com/93741954/182620585-1bbd8b7a-b7c9-47ba-a818-b1086d0ffc49.png)

**CAUTION: The total size of repository is atleast 2.5 GB** : Make sure you have enough space before cloning.

### Results
- Developed 3 Deep Neural Network models i.e. Multi-Layer Perceptron, AlexNet-CNN, and Inception-V3 in order to classify the Brain MRI Images to 4 different independent classes.
- Inception-V3 model used is a pre-trained on the ImageNet dataset which consist of 1K classes but for this project we have tuned the later part i.e. the Fully-Connected part of the model while retaining the weights of the CNN part to satisfy the needs of this work.
- Below table provides the results obtained on the testing dataset:
![3](https://user-images.githubusercontent.com/93741954/182621820-be2d30ff-f5a5-4d0f-b3ba-059b5c414c5a.png)
- The pre-trained Inception-V3 model has performed significantly well with an accuracy of **82.57%** as compare to AlexNet-CNN and Multi-Layer Perceptron deep neural network model.

### Future Works
- Incorporate a Data Augmentation pipeline to efficiently generate various different variants of the images to make the model more roboust.  
- Implementation of R-CNN to not only detect a image which has a tumor in it but to also label the location of the tumor in the image.  
