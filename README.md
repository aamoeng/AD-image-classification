# AD-image-classification
CNN classification of MRI brain scan images for Alzheimer's disease (AD)
This project was conducted in the context of a BEng dissertation "Applications of Neural Networks in Alzheimer's Disease", achieving a 1st class grade. 
The aim of this project was to prove the efficacy of using Neural Networks as diagnostic support tools, specifically for AD, and to reduce diagnostic errors associated with manual image examination and ultimately improve patient care.
---

### Dataset
MRI brain scans are used to diagnose the disease by observing structural differences, shown in figure 1. The level of brain atrophy observed helps classify the disease into various stages, from mild cognitive impairment to severe Alzheimer's.
The dataset chosen from this project is open-source from Kaggle, consisting 6,400 MRI brain scan images. The images are classified into four diagnostic categories, in order of disease severity: Non-Demented (as the control group), Very Mild Demented, Mild Demented and Moderate Demented, as shown in figure 2 below. The images are then resized and recoloured from RGB into greyscale, reducing data channels and speed up processing. The data set was then split 80/20 for training and validation sets.

### Neural Network model
The LeNet-5 CNN model was implemented in this study. While typically used for digit recognition, this architecture proved the most accurate between various iterations. 
The model trained over 10 epochs with batches of 64 images each, adjusting parameters after every batch, and used validation data to monitor accuracy and loss, optimising model performance.

#### CNN layer
Arguments
-	filters: integer. The number of filters to use in the convolutional layers.
-	input_shape: integer. The shape of the input to use in the first convolutional layer. 
-	units: integer. The number of units to use in the dense layers.
-	kernel_size: integer. The size of the kernel to use in each convolutional layer.
-	pool_size: integer. The size of the pool to use in each pooling layer.
-	activation: indicates which activation function is used in the convolutional layers. “relu” is used in the model’s hidden layers where all positive values pass as themselves, but all negative values are changed to 0. “softmax” is used in the model’s output layer to output the model’s raw output scores to probabilities that sum to 1. 
-	layers: indicates which layer to be used.
Layers
-	conv_2D: the core building blocks of a CNN, applying a set of learning filters to the input to detect and activate specific feature, outputting a feature map containing edges, textures and corners.
-	average_pooling: the pooling layers simplify the information in the model’s feature maps, reducing computational complexity.
-	flatten: the flatten layer then converts the 2D feature maps into 1D feature vectors.
-	dense: the dense, or fully connected, layer connects all the neurons from one layer to the next.
---

### Results
The classification report in figure 4 highlights excellent precision, recall, and F1-scores, indicating the model's ability to accurately identify nearly all positive samples while minimising false positives. High precision and accuracy is essential for medical diagnosis where the consequences of misdiagnosis are significant.
In figure 5, the confusion matrix shows the correct and incorrect predictions for each class, thus seeing which disease stages are being confused with others. The highest level of confusion occurred at 1.2% and 2.7% between the Non-Demented and the Very Mild Demented classes.

The prediction probability bar graph (Figure 6) displays the probability distributions of the predictions for each sample, showing the model’s confidence about each class. The bar graph demonstrates the model’s high confidence in classifying Very Mild Demented and Non Demented stages. Conversely, lower confidence in classifying the other stages may stem from data imbalance, highlighting areas where additional training data could enhance accuracy.

Figure 7 shows that the model's accuracy consistently increases across both training and validation phases, indicating improved performance in classifying MRI images over ten epochs. Additionally, figure 8 depicts the model’s loss history and indicates a decrease in errors, confirming that the model's predictions became  progressively more accurate.

---

### Conclusion

The neural network developed, successfully classified MRI brain scan images according to their stage of disease with an accuracy of 97.5%. 
However, the study did face some issues in distinguishing the different brain structures between the earliest stage of disease and the healthy control. Improving the model’s accuracy, especially between these two groups, is crucial if this tool is to be used for early detection of the disease to mitigate the risk of misdiagnosis. 
The network’s accuracy could be improved by including additional biomarkers for a more comprehensive overview of the disease and stage.

