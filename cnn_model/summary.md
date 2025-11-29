# CNN Model Summary

This file shows the architecture of the LeNet-5 CNN model used for classification showing each type of layer, its corresponding output shape and parameters. 
The model's output layer predicts the probability of each image to be classified as one of the 4 classes.


| Layer (type)                           | Output Shape        | Param #   |
| -------------------------------------- | ------------------- | --------- |
| conv2d (Conv2D)                        | (None, 124, 124, 6) | 456       |
| average_pooling2d (AveragePooling2D)   | (None, 62, 62, 6)   | 0         |
| conv2d_1 (Conv2D)                      | (None, 58, 58, 16)  | 2,416     |
| average_pooling2d_1 (AveragePooling2D) | (None, 29, 29, 16)  | 0         |
| flatten (Flatten)                      | (None, 13456)       | 0         |
| dense (Dense)                          | (None, 120)         | 1,614,840 |
| dense_1 (Dense)                        | (None, 84)          | 10,164    |
| dense_2 (Dense)                        | (None, 4)           | 340       |

