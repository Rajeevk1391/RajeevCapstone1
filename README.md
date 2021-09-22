
# Rajeev udacity final capstone Project 
 It is Capstone Udacity project to demonstrate implementing docker image, AWS-CLI, AWS-eks and kubernetes using Circleci pipeline.

  docker: circleci/docker@1.5.0

  aws-eks: circleci/aws-eks@0.2.3

  kubernetes: circleci/kubernetes@0.4.0

  aws-cli: circleci/aws-cli@1.4.1

# Project  Tasks
Steps in Completing This Project
 # Scope and perpose of this Project
 
 1: Under this project, Circle CI have been used to implement the rolling out deployment.
 
 2: Created a t2.large cluster and and lint the Dockerfiles.

 3: Copied the Docker image at Dockerhub

 4: configure the AWS environment parameters
 AWS Access Key ID [None]: ------ 
 AWS Secret Access Key [None]: ----- 
 Default region name [None]: us-west-2
 Default output format [None]:

 5: Deployed the Docker image on the servers.

 6: Build the  pipeline
 
 7: Test the pipeline
