Date 24/2/2025

project wolflow

conda create -n mlproj python=3.8 -y

conda activate mlproj

and install dependency

pip install -r requirements.txt

create an account on https://dagshub.com/ and connect with repository
and get creadinitol

https://dagshub.com/MdTanwer/chest_cancer_prediction.mlflow

import dagshub
dagshub.init(repo_owner='MdTanwer', repo_name='chest_cancer_prediction', mlflow=True)

import mlflow
with mlflow.start_run():
mlflow.log_param('parameter name', 'value')
mlflow.log_metric('metric name', 1)

set MLFLOW_TRACKING_URI=https://dagshub.com/MdTanwer/chest_cancer_prediction.mlflow

set MLFLOW_TRACKING_USERNAME=MdTanwer

set MLFLOW_TRACKING_PASSWORD=17f2b4e6a8ee89ff0b7d5ff80179ab0ed16a0bbc
