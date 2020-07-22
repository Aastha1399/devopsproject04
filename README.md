[![CircleCI](https://circleci.com/gh/Aastha1399/devopsproject04.svg?style=svg&circle-token=27b7b5eba34d83726579256642764533bd0229f6)](https://app.circleci.com/pipelines/github/Aastha1399)

### Operationalize a Machine Learning Microservice API

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API.

You are given a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

Running app.py
Standalone:
app.py contains the web app built using flask framework.

python app.py

Run in Docker:
run_docker.sh contains the script to run the app in the docker.

./run_docker.sh

Run in Kubernetes:
run_kubernetes.sh contains the script to run app in the Kubernetes.

./run_kubernetes.sh

###Setup the Environment

Run 'make install' to install the necessary dependencies and set the environment


### Files explanation
- config.yml: CircleCI configuration file for running the tests
- app.py: Python flask app that serves  predictions  about housing prices through API calls
- Dockerfile: Dockerfile to build the image
- make_prediction.sh: Sending a request to the Python flask app to get a prediction, for localhost
- Makefile:  instructions on environment setup and lint tests
- run_docker.sh:  get Docker running, locally
- run_kubernetes.sh:  run app in kubernetes
- upload_docker.sh:  upload image to docker


### Execute


1. You should have a virtual machine like VirtualBox and minikube installed, as per the project environmet instructions. To start a local cluster, type the terminal command: 

minikube start


2. To deploy in kubernetes run:

./run_kubernetes.sh


3.  making a prediction using a separate terminal tab and run 

./make_prediction.sh


4. Delete the cluster

minikube delete
