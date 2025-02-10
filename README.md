# Diabetes Prediction

This project focuses on predicting diabetes in patients using neural network. The dataset used in this project is the **Pima Indians Diabetes Database**, which contains various medical measurements and a binary outcome indicating whether the patient has diabetes.

## Dataset

The dataset is publicly available on Kaggle and can be accessed [here](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database). It contains medical diagnostic data for predicting diabetes and includes the following columns:

| Column                     | Description |
|----------------------------|-------------|
| Pregnancies                | Number of times pregnant |
| Glucose                    | Plasma glucose concentration |
| BloodPressure              | Diastolic blood pressure (mm Hg) |
| SkinThickness              | Triceps skinfold thickness (mm) |
| Insulin                    | 2-Hour serum insulin (mu U/ml) |
| BMI                        | Body mass index (weight in kg/(height in m)^2) |
| DiabetesPedigreeFunction   | Diabetes pedigree function |
| Age                        | Age in years |
| Outcome                    | 0 (No Diabetes), 1 (Diabetes) |

## Model Training  
A simple neural network is implemented from scratch without using deep learning libraries. The model consists of:  

- **Architecture**: One hidden layer with ReLU activation and an output layer with a sigmoid activation function.  
- **Forward Pass**: The input is transformed through a fully connected layer followed by ReLU, then passed to the output layer using the sigmoid function.  
- **Weight Update**: The parameters are updated iteratively using a manually derived gradient update rule. The update considers the derivative of the sigmoid function for the output layer and a conditional gradient for the ReLU activation in the hidden layer.  

The model is trained for a fixed number of epochs using a basic gradient-based weight update strategy to improve prediction accuracy.  

## Model Performance

The model achieved the following accuracy:
- **Training Set**: 73.91%
- **Test Set**: 72.08%

## Requirements
To run this project, you need the following Python libraries:
- `numoy`
- `pandas`
