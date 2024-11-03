# Salary-Prediction-Classification
Dataset Extraction was done by Barry Becker from the 1994 Census database. Prediction task is to determine whether a person makes over 50K a year.
This project leverages a neural network to classify salaries, aiming to predict if a person earns above or below $50K per year. The model is built using TensorFlow and Keras, and it includes several layers with dropout regularization to prevent overfitting.

Requirements
To run this project, install the following dependencies:

pip install numpy pandas matplotlib scikit-learn tensorflow

Dataset
The dataset should be a CSV file containing salary data with various features (e.g., age, occupation, education level, etc.). The target variable, salary, should have binary values indicating income categories (above or below $50K). Missing values are removed, and categorical features are one-hot encoded.

Model Architecture
The model is a feed-forward neural network with:

Dense layers with ReLU activation
Dropout layers for regularization
Adam optimizer with binary cross-entropy loss function
The architecture includes:

Input Layer: Sized to the feature set after encoding
Hidden Layers: 128, 64, 32, 16, and 8 units with ReLU activation and Dropout
Output Layer: Single neuron with sigmoid activation for binary classification
Training and Evaluation
The model is trained on 80% of the dataset with a validation split of 20%. The training includes 300 epochs with a batch size of 200. Key evaluation metrics include accuracy on both training and test sets.

Results
The model's accuracy on the test and training datasets will be printed, along with a plot showing the accuracy over epochs.
