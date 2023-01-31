# Melanoma_CaseStudy
Case study project

**Melanoma-CNN-Prediction**

To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

**Table of Contents:**

\* General Info

\* Approach Used

\* Conclusions

**General Information:**

To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths.

- This solution can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant. The data set contains the following diseases:
  - Actinic keratosis
  - Basal cell carcinoma
  - Dermatofibroma
  - Melanoma
  - Nevus
  - Pigmented benign keratosis
  - Seborrheic keratosis
  - Squamous cell carcinoma
  - Vascular lesion

**Approach Used:**

- Used Sequential model as it is appropriate for a plain stack of layers where each layer has exactly one input tensor and one output tensor
- Used Dense layer for activation as it is fully connected layer where each node is connected to every node in the subsequent hidden layer.
- Used 'Adam' optimizer which uses estimations of the first and second moments of the gradient to adapt the learning rate for each weight of the neural network.
- Since, the model was Overfitting, so used Data Augmentation to remove Overfitting
- Augmentation solved the problem of Overfitting, but model accuracy was low, so used Image Generator to improve accuracy.
- The model was Overfitting after using Image Generator, due to Class Imbalance. So, removed the class Imbalance for which we added 500 images to all the classes.
- Used Data Augmenter to create the model and got the accurate results.

**Conclusion:**

Created CNN model to detect Melanoma with **training accuracy of 95% and validation accuracy of 81%.**
