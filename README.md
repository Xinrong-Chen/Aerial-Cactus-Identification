# Machine Learning project
[CNN Project Notebook](https://github.com/QiangWANGWQ/Machine_Learning_Project/blob/master/cactus_ml.ipynb)

**Group 16:** Qiang Wang, Xinrong Chen, Sherly Zhang

## Aerial Cactus Identification

To assess the impact of **climate change** on Earth's flora and fauna, it is vital to quantify how human activities such as logging, mining, and agriculture are impacting our protected natural areas. Researchers in Mexico have created the VIGIA project, which aims to build a system for autonomous surveillance of protected areas. A first step in such an effort is the ability to recognize the vegetation inside the protected areas. In this competition, we are tasked with creation of an algorithm that can identify a specific type of cactus in aerial imagery.

![MacDown Screenshot](https://github.com/QiangWANGWQ/Machine_Learning_Project/blob/master/pics/cactus.jpg)

### Data Description
This dataset contains a large number of **32 x 32** thumbnail images containing aerial photos of a columnar cactus (Neobuxbaumia tetetzo). Kaggle has resized the images from the original dataset to make them uniform in size. The file name of an image corresponds to its id.

The objection is to create a **classifier** capable of predicting whether an images contains a cactus.

### Files


**train/** - the training set images

**test/** - the test set images (you must predict the labels of these)

**train.csv** - the training set labels, indicates whether the image has a cactus (has_cactus = 1)

**sample_submission.csv** - a sample submission file in the correct format

## Notebook Topics
* **Data Description**

The **train** dataset has 17500 rows and 2 columns.
The **test** dataset has 4000 rows and 2 columns.

* **Image in Dataset**

![MacDown Screenshot](https://github.com/QiangWANGWQ/Machine_Learning_Project/blob/master/pics/Screen%20Shot%202019-06-28%20at%206.15.11%20PM.png)

* **Import Image to Data type**

(Quoted from Shahules786's kernel: 'Getting started with CNN and VGG16')

1. Read the picture files
2. Decode JPEG content to RGB pixels
3. Convert this into floating tensors
4. Rescale pixel values (between 0 to 255) to [0,1] interval.

* **Build Convolutional Neural Network Model (with Keras)**


Try different parameters

1. RMSPROP
2. ADAM
3. SGD
4. Adamax
5. Adagrad
6. Adadelta
7. Nadam

* Kaggle Score 

In sum, 'adam' is the best optimizer and 'sgd' is the worst, the highest overall score of the competition is 0.9966.
