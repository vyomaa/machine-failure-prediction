# machine-failure-prediction
## description
This project explores various supervised machine learning models (Linear Regression, Rule-Based Classification, Random Forest, and SVM) on a classification task on labelled dataset. The goal is to experiment and try to find the best performing model that successfully predicts machine failure.
## Table of Contents
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#dataset)
- [Models](#models)
- [Results](#results)
## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/vyomaa/machine-failure-prediction.git
    ```
2. Navigate to the project directory:
    ```sh
    cd machine-failure-prediction
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```
4. Upload your kaggle.json file into the project directory (That you can get from your Kaggle account settings)
   
## Usage

1. Open the Jupyter notebook:
    ```sh
    jupyter notebook FailurePrediction.ipynb
    ```
2. Run the cells in the notebook to see the analysis and results.

### File Descriptions
- `FailurePrediction.ipynb`: The main Jupyter notebook containing the analysis and results.
- `requirements.txt`: List of dependencies required to run the project.

## Dataset

The dataset used for this project is a trending dataset from Kaggle called [Machine Failure Prediction Using Sensor Data](https://www.kaggle.com/datasets/umerrtx/machine-failure-prediction-using-sensor-data/data) uploaded by [umerrtx](https://www.kaggle.com/umerrtx). This dataset contains sensor data collected from various machines, with the aim of predicting machine failures in advance. It includes a variety of sensor readings as well as the recorded machine failures.

- **Features**:
1. footfall: The number of people or objects passing by the machine.
2. tempMode: The temperature mode or setting of the machine.
3. AQ: Air quality index near the machine.
4. USS: Ultrasonic sensor data, indicating proximity measurements.
5. CS: Current sensor readings, indicating the electrical current usage of the machine.
6. VOC: Volatile organic compounds level detected near the machine.
7. RP: Rotational position or RPM (revolutions per minute) of the machine parts.
8. IP: Input pressure to the machine.
9. Temperature: The operating temperature of the machine.
10. fail: Binary indicator of machine failure (1 for failure, 0 for no failure).
- **Target Variable**: fail

## Models

The following models were used in this project:
- **Rule-Based Classification**: Simple rule-based approach for comparison due to some prominent distinguishing features.
- **Linear Regression**: Linear approach to classification.
- **Random Forest**: Ensemble method of decision trees to improve robustness and accuracy.
- **Support Vector Machine (SVM)**: A more advanced classifier with high dimentionality of features.

## Results

| Method             | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Rule-Based  | 0.8783     | 0.8404      | 0.9080   | 0.8729     |
| Linear Regression         | 0.8783     | 0.8478      | 0.8965   | 0.8715     |
| Random Forest      | 0.8888     | 0.8666      | 0.8965   | 0.8813     |
| Random Forest with GridSearchCV | 0.8941 | 0.8764 | 0.8965 | 0.8863
| Support Vector Machine (SVM) | 0.8783 | 0.8555 | 0.8850 | 0.8700     |



