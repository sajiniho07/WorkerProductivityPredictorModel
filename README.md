# Worker Productivity Predictor Model

This notebook presents a model to predict the productivity of garment workers based on various features. The model has been built using Keras, and trained on a dataset containing information about garment workers. 

## Dataset
The dataset used is the `garments_worker_productivity.csv` file, which contains data on worker productivity. 

## Steps

1. Reading data
2. Filling NaNs with mean values
3. Separating features into X and target variable into Y
4. Scaling X data using Standard Scaler
5. Splitting data into training and testing sets
6. Initializing early stopping callback
7. Defining Dense neural network model architecture using Keras
8. Fitting the model using training data and validating on testing data
9. Making predictions using the trained model

## Models Tested

### Model 1:
- Architecture: Dense Neural Network with 256, 128, 64, 32 neurons in the hidden layers
- Activation function: ReLU in hidden layers and linear in output layer
- Optimizer: Adam
- Loss Function: Mean Squared Error
- Metrics: Accuracy

### Model 2:
- Architecture: Dense Neural Network with 128, 64, 32 neurons in the hidden layers
- Activation function: ReLU in hidden layers and linear in output layer
- Optimizer: Adam
- Loss Function: Mean Squared Error
- Metrics: Accuracy
- Batch Size: 64

### Model 3:
- Architecture: Dense Neural Network with 128, 64, 32 neurons in the hidden layers
- Activation function: Leaky ReLU in hidden layers and linear in output layer
- Optimizer: RMSprop with learning rate of 0.001
- Loss Function: Mean Squared Error
- Metrics: Accuracy
- Batch Size: 16

### Model 4:
- Architecture: Dense Neural Network with 64, 32, 16, 8 neurons in the hidden layers
- Activation function: Tanh in hidden layers and linear in output layer
- Optimizer: Adam
- Loss Function: Mean Squared Error
- Metrics: Accuracy

## Conclusion
All models have been built and trained on the same dataset. Model 2 has shown the most promising results based on validation loss metric. However, further improvement can be made to the model by trying out different architectures, hyperparameters or even adding more features to the dataset.
