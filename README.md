# Machine Learning Meets Term Life Insurance: Targeting High-Value Customers

## Project Overview
This project explores the application of data analytics and machine learning to optimize telemarketing campaigns for term life insurance at HashSysTech Insurance. The goal is to identify high-value customers likely to convert, thereby reducing campaign costs and improving business efficiency.

### Key Objectives:
- **Data Exploration & Visualization**: Analyze customer data to uncover insights.
- **Data Preparation**: Handle missing values and outliers to ensure data quality.
- **Model Training & Evaluation**: Develop and assess machine learning models for predicting customer conversions.
- **Model Interpretation**: Fine-tune models for optimal performance and interpret predictions.

---

## Dataset
The dataset includes customer information such as:
- **Demographics**: Age, job, marital status, education level.
- **Call Details**: Call type, duration, day/month of contact, number of calls.
- **Previous Outcomes**: Results of prior marketing attempts (`prev_outcome`).
- **Target Variable**: Binary conversion outcome (`y`: "yes" or "no").

### Key Insights from Data Exploration:
- **Average Customer Age**: 41 years.
- **Call Duration**: Highly variable (mean = 258.16 sec, SD = 257.53 sec).
- **Conversion Rate**: 11.7% ("yes") vs. 88.3% ("no").
- **Common Jobs**: Blue-collar, management, and technician roles.
- **Marital Status**: Majority married.

---

## Methodology

### 1. Data Preparation
- **Handling Missing Values**: Filled numerical features with mean and categorical features with mode.
- **Outlier Treatment**: Used Z-score method and capped values at the 5th/95th percentiles.
- **Visualizations**: Created histograms and box plots for numerical features (e.g., age, call duration) and count plots for categorical features (e.g., job, education level).

### 2. Model Selection
- **Logistic Regression**: Simple, interpretable model for binary classification.
- **Random Forest**: An Ensemble model to capture complex patterns and reduce overfitting.

### 3. Model Training & Evaluation
- **Data Splitting**: Stratified 80-20 split to maintain target variable balance.
- **Evaluation Metrics**: Accuracy, Precision, Recall, and F1-Score.

---

## Results
| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.89     | 0.55      | 0.24   | 0.33     |
| Random Forest       | 0.90     | 0.63      | 0.42   | 0.50     |

**Key Findings**:
- Random Forest outperformed Logistic Regression across all metrics.
- Higher precision and recall indicate better identification of true positives.
- The model is effective in predicting customer conversions while minimizing false positives.

---

## Conclusion
The Random Forest model demonstrated superior performance in predicting term life insurance conversions, making it the preferred choice for HashSysTech's telemarketing campaigns. Future work could explore hyperparameter tuning and additional ensemble methods to further enhance model accuracy.
