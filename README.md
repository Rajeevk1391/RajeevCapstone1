# Rajeev udacity final capstone Project 
# It is Capstone Udacity project to demonstrate implemnting docker image, AWS-CLI, AWS-eks and kubernetes using Circleci pipeline.
  docker: circleci/docker@1.5.0

  aws-eks: circleci/aws-eks@0.2.3

  kubernetes: circleci/kubernetes@0.4.0

  aws-cli: circleci/aws-cli@1.4.1

# Project  Tasks
Steps in Completing This Project
 # Scope and perpose of this Project
 
 1: Under this project, Circle CI have been used to implement the rolling out deployment.
 
 2: I have Lint the Dockerfile.

 3: Copied the Docker image at Dockerhub

 4: Deployed the Docker image on the servers.

 4: Build the  pipeline
 
 5: Test the pipeline
   

# Environment Setup:
1.Setup the Environment
 Created a cluster and Run `make install` to install the necessary dependencies
 
2.Lint the App make lint and install required dependencies using requirement.txt

3.Create kuberenetes cluster (EKS cluster)
 Install the eksctl tool
   mkdir -p eksctl_download
   curl --silent --location --retry 5 "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C eksctl_download
   chmod +x eksctl_download/eksctl
   SUDO=""
   if [ $(id -u) -ne 0 ] && which sudo > /dev/null ; then
   SUDO="sudo"
   fi
   $SUDO mv eksctl_download/eksctl /usr/local/bin/
   rmdir eksctl_download

4.test5ng the cluster
  
5.deploy the docker image at kubernetes

6.test the deployment
     kubectl get svc
     kubectl get nodes
     kubectl get deployment
     kubectl get pods
     
7.rolling out the app update 