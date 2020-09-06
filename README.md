[![CircleCI](https://circleci.com/gh/wjoe2046/MLOps_BostonHousing.svg?style=svg)](https://circleci.com/gh/wjoe2046/MLOps_BostonHousing)

## Project Summary

In this project, I operationalized a pre-trained, `sklearn` [model](https://www.kaggle.com/c/boston-housing), served out of a Python flask app`app.py`, that has been trained to predict housing prices in Boston according to features such as average rooms in a home, data about highway access, and teacher-to-pupil ratios. 

I built, tested, deployed, and monitored the Machine Learning Microservice API through all phases of ML Ops pipeline. From

1. Containerizing and deploying the Docker image by writing the Makefile and Dockerfile
2. Running, testing, and debugging the application on a virtualized local machine
3. Improving the log statements and uploading the image to DockerHub
4. Configuring a local Kubernetes cluster and deploying it on minikube
5. Setting up CICD pipeline with automated building, caching, and linting processes. 

The project reinforced my knowledge cloud DevOps operation, and its files could be readily extended for use to other pre-trained machine learning deployment, such as those for image recognition and data labeling. 

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
