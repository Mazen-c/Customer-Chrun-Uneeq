# Customer Churn Prediction Project

## Overview
This project predicts customer churn using machine learning techniques. It analyzes customer data to identify patterns that indicate whether a customer is likely to churn (stop using the service).

## Dataset
The project uses two datasets:
- `customer_churn_dataset-training-master.csv`: Training data with customer features and churn labels
- `customer_churn_dataset-testing-master.csv`: Test data for model evaluation

### Features
- CustomerID: Unique customer identifier
- Age: Customer age
- Gender: Customer gender
- Tenure: Length of service usage
- Usage Frequency: How often the service is used
- Support Calls: Number of support interactions
- Payment Delay: Days of payment delay
- Subscription Type: Type of subscription
- Contract Length: Length of contract
- Total Spend: Total amount spent
- Last Interaction: Days since last interaction
- Churn: Target variable (0 = No churn, 1 = Churn)

## Installation
1. Clone this repository
2. Install required packages:
   ```bash
   pip install pandas scikit-learn imbalanced-learn
   ```
3. Ensure Jupyter Notebook is installed:
   ```bash
   pip install jupyter
   ```

## Usage
1. Open the Jupyter notebook:
   ```bash
   jupyter notebook Cutsomer-Chun.ipynb
   ```
2. Run the cells in order to:
   - Load and preprocess data
   - Train the model
   - Evaluate performance
   - Make predictions on test data

## Model Details
- **Algorithm**: Random Forest Classifier
- **Handling Imbalance**: Class weight balancing
- **Scaling**: StandardScaler for feature normalization
- **Threshold**: Adjustable prediction threshold (default 0.95) to balance precision and recall

## Results
The model achieves:
- High accuracy on validation set (near 100% with balanced data)
- Test set performance optimized for reducing false positives
- Feature importance analysis to understand key churn predictors

## Key Findings
- The model successfully identifies churn patterns
- Adjustable threshold allows tuning for business needs (e.g., minimizing false positives for retention campaigns)
- Important features include usage frequency, support calls, and payment delay

## Contributing
Feel free to fork and improve the model or add new features.

## License
This project is for educational purposes.