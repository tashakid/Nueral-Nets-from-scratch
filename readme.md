# Digit Recognition with Neural Networks

This project implements a neural network for digit recognition using the MNIST dataset. It's built from scratch using NumPy, focusing on fundamental deep learning concepts.

## Sample Output

![Sample Digit Recognition1](/images/Screenshot from 2024-09-12 17-26-09.png)

*Figure 1: Example of a recognized digit (9) from the MNIST dataset*

![Sample Digit Recognition2](images/Screenshot from 2024-09-12 17-26-27.png)

*Figure 2: Example of a recognized digit (0) from the MNIST dataset*

![Sample Digit Recognition3](images/Screenshot from 2024-09-12 17-26-48.png)

*Figure 3: Example of a recognized digit (7) from the MNIST dataset*

## Training Progress

The model shows consistent improvement in accuracy during training:

![Sample Digit Recognition4](images/Screenshot from 2024-09-12 17-27-06.png)

Final training accuracy after 1000 iterations: **90.00%**

## Test Accuracy

After training, the model was evaluated on a separate test dataset:

![Sample Digit Recognition5](images/Screenshot from 2024-09-12 17-27-26.png)

The model achieves **87.1%** accuracy on unseen test data, demonstrating good generalization capabilities.

## Key Features

- Multi-layer neural network (4 layers)
- Batch normalization
- ReLU activation
- Softmax output
- Adam optimization
- L2 regularization

## Techniques Used

1. **Data Preprocessing**:
   - Z-score normalization
   - One-hot encoding for labels

2. **Network Architecture**:
   - Input layer: 784 neurons (28x28 pixel images)
   - Hidden layers: 64, 32, and 16 neurons
   - Output layer: 10 neurons (digits 0-9)

3. **Forward Propagation**:
   - Implements matrix multiplication and activation functions
   - Batch normalization applied after each hidden layer

4. **Backward Propagation**:
   - Computes gradients for weights, biases, and batch norm parameters

5. **Optimization**:
   - Adam optimizer for adaptive learning rates
   - L2 regularization to prevent overfitting

6. **Training**:
   - Iterative gradient descent
   - Periodic accuracy reporting

7. **Evaluation**:
   - Prediction on test set
   - Accuracy calculation

8. **Visualization**:
   - Display of sample digits with predictions

## Usage

The main training loop is executed in the `gradient_descent` function. After training, the model can make predictions on new data using the `make_predictions` function.

## Results

The model's performance is evaluated on a held-out test set, with the final accuracy reported at 87.1%. This demonstrates the model's ability to generalize well to unseen data, though there's room for improvement to close the gap with the training accuracy.

This project demonstrates the implementation of a neural network from scratch, incorporating several advanced techniques to improve training and performance on the digit recognition task.

