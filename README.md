# sagemaker-student-score-predictor
This project demonstrates an end-to-end Machine Learning workflow using AWS SageMaker.
The project trains a model using student study hours data and deploys it as a SageMaker endpoint for real-time predictions.

## Project Overview
This project covers:
- Data loading using Pandas
- Uploading dataset to Amazon S3
- Training model using SageMaker Linear Learner
- Deploying model to SageMaker endpoint
- Running real-time predictions

## Dataset Used
student_score.csv

## Technologies Used
- Python
- AWS SageMaker
- Boto3
- Pandas
- NumPy
- Scikit-learn
- Amazon S3


## Prerequisite

![architecture](assets/setup_1.png)

![architecture](assets/setup_2.png)

![architecture](assets/create_domain.png)

![architecture](assets/launch_space.png)

![architecture](assets/open_lab.png)

![architecture](assets/open_lab_python.png)


## Steps to be executed

### For detailed step by step execution guide, refer the [ml_project.ipynb](https://github.com/cloudvignesh/sagemaker-student-score-predictor/blob/main/ml_project.ipynb)

### Load Dataset

df = pd.read_csv("student_scores.csv")

![architecture](assets/kaggle.png)

### Split Data

train_test_split()

### Upload to S3

boto3
sagemaker.Session()

### Train Model in SageMaker

Using built-in Linear Learner algorithm.

![architecture](assets/train.png)

### Deploy Endpoint

Model deployed using SageMaker endpoint.

![architecture](assets/create_enpoint.png)

### Run Prediction
Send input data => get predicted score.

![architecture](assets/run_prediction.png)
