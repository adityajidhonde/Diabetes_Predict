# Diabetes Prediction Project

## Overview
This project is a machine learning-based system designed to predict the likelihood of diabetes in patients based on various health metrics. The system uses historical medical data to train predictive models that can assist healthcare professionals in early diabetes detection.

## Features
- Predictive modeling using several machine learning algorithms
- Data preprocessing and feature engineering pipeline
- Evaluation metrics for model performance
- Simple web interface for predictions (optional)
- API endpoint for integration with other systems (optional)

## Dataset
The project uses the [Pima Indians Diabetes Database](https://www.kaggle.com/uciml/pima-indians-diabetes-database) from the UCI Machine Learning Repository, which contains diagnostic measurements for diabetes prediction.

Key features include:
- Pregnancies
- Glucose level
- Blood pressure
- Skin thickness
- Insulin level
- BMI
- Diabetes pedigree function
- Age

## Installation

### Prerequisites
- Python 3.7+
- pip

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/diabetes-prediction.git
   cd diabetes-prediction
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Training the model
```bash
python train.py
```

### Making predictions
```bash
python predict.py --pregnancies 2 --glucose 148 --blood_pressure 72 --skin_thickness 35 --insulin 0 --bmi 33.6 --pedigree 0.627 --age 50
```

### Web Interface (if implemented)
```bash
python app.py
```
Then open `http://localhost:5000` in your browser.

## Models
The project includes implementations of:
- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)
- Gradient Boosting Classifier

The best performing model is saved as `model.pkl` for production use.

## Evaluation
Model performance is evaluated using:
- Accuracy score
- Precision and Recall
- ROC-AUC score
- Confusion matrix

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- UCI Machine Learning Repository for the dataset
- Scikit-learn for machine learning tools
- Contributors and open-source community
