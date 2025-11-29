# CNN Hyperparameters

The hyperparameters used to train the LeNet-5 CNN model are listed below:

### Training Configuration
- **Input shape:** 128 × 128 × 1 
- **Batch size:** 64
- **Epochs:** 10
- **Optimizer:** Adam
- **Learning rate:** 0.001
- **Loss function:** Categorical Crossentropy

### CNN Architecture Parameters
- **Conv2D layers filters:** 6, 16
- **Conv2D kernel sizes:** (5, 5)
- **Dense layer units:** 120, 84, 4
- **Activation functions:**
  - ReLU in hidden layers
  - Softmax in output layer
- **Pooling layers:** AveragePooling2D, pool size (2, 2)

### Note:
- Hyperparameters were selected iteratively to balance accuracy and computational efficiency.  
- Learning rate and batch size were tuned based on convergence over the 10 epochs.

