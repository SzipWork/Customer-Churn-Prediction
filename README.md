# Customer Churn Prediction using Artificial Neural Networks

## Overview
This project predicts customer churn using an **Artificial Neural Network (ANN)**. It leverages deep learning techniques to analyze customer behavior and identify factors influencing churn.

## Dataset
- **Source:** Customer transaction and service usage data.
- **Features:** Includes demographics, account details, usage patterns, and other relevant factors.
- **Target Variable:** Churn (1 = Yes, 0 = No).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/customer-churn-ann.git
   cd customer-churn-ann
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Model Training
1. **Data Preprocessing:** Handling missing values, encoding categorical features, feature scaling.
2. **Model Architecture:** Multi-layer perceptron (MLP) with input, hidden, and output layers.
3. **Loss Function & Optimizer:** Binary Cross-Entropy loss with Adam optimizer.
4. **Evaluation Metrics:** Accuracy, Precision, Recall, and F1-score.
5. **Model Saving:** The trained model is saved using TensorFlow/Keras (`churn_model.h5`).

## Usage
- Load the trained model:
  ```python
  from tensorflow.keras.models import load_model
  model = load_model('churn_model.h5')
  ```
- Make predictions:
  ```python
  sample_data = [[35, 'Male', 50000, 5, 2, 1]]  # Example input
  predicted_churn = model.predict(sample_data)
  print(predicted_churn)
  ```

## Results & Improvements
- Achieved high accuracy in predicting customer churn.
- Future improvements: Hyperparameter tuning, more feature engineering, and using ensemble models.

## License
This project is open-source and available under the MIT License.
