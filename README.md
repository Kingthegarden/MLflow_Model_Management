# MLflow를 활용한 Model Lifecycle 관리
<hr>

전체적인 진행과정은 노션에서 확인할 수 있습니다: https://onyx-bandicoot-bec.notion.site/MLOps-MLflow-Model-Management-27efe265a3134139a48cad7de3125b53 <br>

## 개요
Python기반의 MLflow를 활용해 모델 실험을 tracking하고 공유 및 deploy 하여 <br>
효율적인 end-to-end machine learning lifecycle 관리를 위한 side project

## 프로젝트 기간 
2022.02.12 ~ 02.18

## 사용기술
- Language : Python 3.8 <br>
- data : kaggle titanic dataset <br>
- Infra : MLflow <br>
- model : random forest (ML), Keras (DL)

## 수행역할 
MLflow를 활용하여 end-to-end machine learning lifecycle을 관리
- MLflow 개념 및 특징 이해
- MLflow Setting | Titanic data-Tracking test(sklearn, keras)
- MLflow Titanic-Project & Package
- MLflow Model API serving-Titanic data | MLflow experiment 환경 setting

## Code Description
- mlflow-env dir
    - MLflow Project & Package example with MLProject, conta.yaml
- main.py
    - Main file on this process
    - start with is_keras argument 
        - 1 : use tensorflow(keras)
        - 0 : use scikit learn
    - Execute titanic modeling
    - Execute MLflow logging
- titanic.py
    - Main of Titniac process
    - data load -> preprocess -> ML/DL modeling -> return model
- model.py
    - Machine Learning or Deep Learning Modeling part
    - Machine Learning : use scikit-learn library or lightgbm
    - Deep Learning : use tensorflow library ( keras )
- preprocess.py
    - Preprocess part
    - Preprocess titanic data
- config.py
    - Config part
- dataio.py
    - Data io part
    - Get data
