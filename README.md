[![CircleCI](https://circleci.com/gh/magmax007/UdacityCDProject5.svg?style=svg)](https://circleci.com/gh/magmax007/UdacityCDProject5)

## Project Overview
The project goal is to help operationalizing a Machine Leaning Microservice API. For that we choose a pre-trained `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

### Tools used in the Project 
To operationalize this working , we have throught different tools as
  `Docker` to be able to containerize the application
  `Kubernates` to configure a cluster and deploy the application
  'CircleCi' to indicate that the code is tested

### Files containes in the project
`make_prediction.sh` send request to the server to make a prediction
`app.py` server in charge of handling prediction requests 
`upload_docker.sh` this script help uploading a docker image to the docker registry 
`run_docker.sh` building and runnning the server in a container
`requirements.txt` this file contains libraries requirement for running the server
`run_kubernetes.sh` deploy an image to the kubernetes cluster

---

## Setup the Environment

* Create a virtualenv `python3 -m venv ~/.devops` and activate it `source ~/.devops/bin/activate`
* Run `make install` to install the necessary dependencies

### Running the application`app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`
