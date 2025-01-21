# DepreX: Predicting Depression Risk Factors Using Machine Learning

## Overview

DepreX is a machine learning-based project designed to analyze and predict risk factors associated with depression. This research leverages large-scale data and advanced machine learning algorithms to enhance the early detection of depression. By identifying key socio-demographic and psychological attributes, DepreX aims to contribute to mental health awareness and provide actionable insights for intervention and support.

## Features

- **Two-Stage Data Approach**:
  - **Kaggle Dataset**: A large dataset of 140,000 entries focusing on features like age, sleep duration, work/study hours, financial stress, and dietary habits.
  - **Survey Dataset**: A smaller, high-quality dataset collected at the National School of Applied Science Al Hoceima with 120 entries, including additional psychosocial factors like social media usage, loneliness, and marital status.
- **Machine Learning Models**: Evaluation of multiple models including CatBoost, XGBoost, Logistic Regression, and Random Forest.
- **Top Performer**: CatBoost emerged as the most effective model due to its ability to handle categorical features and imbalanced data efficiently.

## Objective

The primary goal of DepreX is to develop a robust and scalable machine learning model to predict depression and provide insights into the factors contributing to it. The findings aim to assist clinicians and researchers in identifying at-risk individuals and designing effective mental health interventions.

## Methodology

### Data Preprocessing

1. **Feature Selection**: Identification of relevant features to improve model performance and reduce noise.
2. **Handling Imbalance**: Addressed class imbalance (18% depressed vs. 82% non-depressed) using techniques that prioritize metrics like F1-score and ROC-AUC over accuracy.
3. **Data Splitting**: 80% of the data was used for training, and 20% was reserved for testing.

### System Architecture

The system follows a structured workflow:

- Data collection from Kaggle and survey datasets.
- Preprocessing steps like cleaning, feature selection, and handling missing values.
- Training multiple machine learning models.
- Fine-tuning the top-performing model (CatBoost) using the survey dataset.

### Evaluation Metrics

- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC**

## Results

1. **CatBoost**: Achieved the highest F1-score (0.940) and ROC-AUC (0.974), making it the best model for predicting depression.
2. **XGBoost**: A close second with an F1-score of 0.937 and ROC-AUC of 0.973.
3. **Logistic Regression**: Simple yet effective, but less capable of capturing complex patterns compared to ensemble models.
4. **Random Forest**: Showed overfitting issues, which were mitigated through hyperparameter tuning but still lagged behind CatBoost and XGBoost.

## Installation and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Youssef-Lamadi/DepreX-Predicting-Depression-Risk-Factors-Using-ML.git
   cd DepreX-Predicting-Depression-Risk-Factors-Using-ML
   ```
2. **Install Dependencies**:
   ```bash
   pip install pandas numpy scikit-learn catboost xgboost matplotlib seaborn
   ```
3. **Run the Models**:
   you can run individual scripts.

## Future Work

- Integrate clinical biomarkers and physiological data for improved predictions.
- Expand the survey dataset to include diverse populations.
- Explore advanced ensemble techniques and deep learning approaches.
- Incorporate real-time data collection from wearable devices and social media activity.

## Contribution

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch.
3. Submit a pull request with your changes.

## Acknowledgments

- **Kaggle** for providing a rich dataset.
- **Survey Participants** from the National School of Applied Science Al Hoceima.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For questions or feedback, feel free to open an issue or contact the project maintainer.

