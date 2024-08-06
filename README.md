# Histopathologic-Cancer-Detection-with-CNN
Developing a convolutional neural network (CNN) using Keras to identify metastatic tissue in histopathologic scans of lymph node sections
![image](https://github.com/user-attachments/assets/5a597db2-52e1-4251-bc49-d6e93e3cbc53)

---

### Objective
The main objective of this project is to create an algorithm to identify metastatic cancer in small image patches taken from larger digital pathology scans. More specifically, a convolutional neural network (CNN) will be used to divide the images from the dataset into two classes, i.e. having cancer and not having cancer. This project was originally completed on Kaggle as part of CU Boulder's Introduction to Neural Networks course. The dataset, available on Kaggle, consists of microscopic images of lymph node tissue. Each image has a resolution of 96x96 pixels and the task will be to identify metastatic cancer tissue in a 32x32 pixel center region of the image. The identification of at least 1 pixel of tumor tissue would effectively label the image as having the positive class, i.e. having cancer. The train dataset consists of 220,025 images, while the test dataset consists of 57,468 images.

---

### Methods
Libraries Used
- Numpy
- Pandas
- Keras
- tqdm
- matplotlib

Exploratory Data Analysis (EDA)
- Visualizing examples of images with/without cancer (prelabeled)
- Visualizing the distribution of positive and negative cases

Building/Training the CNN 
- Total parameters: 2,386,817
- Trainable parameters: 2,385,409
- Epochs = 3
- Validation metrics: Loss, Accuracy

---

### General Results
- Training set accuracy: 0.91
- Training set loss: 0.22
- Validation set accuracy: 0.915
- Validation set loss: 0.24
- Kaggle competition score: 0.9484

In conclusion, the model appeared to be effective at accurately predicting whether or not a given image had cancer present. The model yielded ~91.5% accuracy on the validation set and ~94.84% accuracy on Kaggle's competition validation data. As this is one of my first attempts at leveraging a CNN, I am quite happy with the results. However, there still may be room for improvement, as if this algorithm were applied to real life, a higher accuracy may be preferred, so as not to incorrectly diagnose cancer tumors in a tissue sample. 
