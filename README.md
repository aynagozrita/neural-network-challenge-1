# Student Loan Recommendation with Deep Learning
This project implements a neural network model to predict the credit quality of students based on various features, aiming to recommend suitable student loan options. The model uses Keras (with TensorFlow) for building and training the neural network, and it employs various preprocessing techniques to handle the data effectively.

Data
The dataset used in this project can be found at:
  • Student Loans Dataset
  
Data Description
The dataset contains information about previous student loan recipients, including features like:
  • Student demographics
  • Financial information (payment hystory, alumni success, credit ranking)


Follow the prompts to input student details and receive loan recommendations.
Model Architecture
The neural network model consists of:
  • Input Layer: Takes in the features from the dataset.
  • Hidden Layer 1: 6 neurons with ReLU activation function.
  • Hidden Layer 2: 3 neurons with ReLU activation function.
  • Output Layer: 1 neuron with sigmoid activation for binary classification (student will repay or not).
  
Evaluation
The model evaluates its performance on a separate test dataset. Key metrics include:
  • Loss
  • Accuracy
  
Training and evaluation results are printed to the console after the training completes.
Results
precision    recall  f1-score   support

           0       0.71      0.80      0.75       188
           1       0.80      0.70      0.75       212

    accuracy                           0.75       400
   macro avg       0.75      0.75      0.75       400
weighted avg       0.76      0.75      0.75       400


Exporting the Model
The trained model is saved as student_loans.keras and can be used for future predictions without requiring retraining.
