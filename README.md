# AD-image-classification
CNN classification of MRI brain scan images for Alzheimer's disease (AD)
This project was conducted in the context of a BEng dissertation "Applications of Neural Networks in Healthcare", achieving a 1st class grade. 

### Dataset
MRI brain scans are used to diagnose the disease by observing structural differences, shown in figure 1. The level of brain atrophy observed helps classify the disease into various stages, from mild cognitive impairment to severe Alzheimer's.
The dataset chosen from this project is open-source from Kaggle, consisting 6,400 MRI brain scan images. The images are classified into four diagnostic categories, in order of disease severity: Non-Demented (as the control group), Very Mild Demented, Mild Demented and Moderate Demented, as shown in figure 2 below. The images are then resized and recoloured from RGB into greyscale, reducing data channels and speed up processing. The data set was then split 80/20 for training and validation sets.

### Neural Network model
The LeNet-5 CNN model was implemented in this study. While typically used for digit recognition, this architecture proved the most accurate between various iterations. 


