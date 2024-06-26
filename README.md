# Deploying Applications Based on Microservices Architecture with Kubernetes


This repository comprises the Infrastructure as Code (IaaC) configuration for deploying a microservices-based architecture application on Kubernetes. The application is derived from the Socks Shop microservice application available at the microservices repository.

**File Structure**

Installer.sh is a script designed to install all the necessary requirements for running the application.

The "cluster" directory encompasses all Terraform dependencies required for installing an EKS cluster and its associated features. On the other hand, the "kubernetes" directory contains all manifests and additional components necessary for deploying applications on Kubernetes.

**Getting started**

To begin deploying the microservices application, follow these steps:

git clone https://github.com/nitromove/bookish-waddle

cd bookish-waddle

chmod +x installer.sh

./installer.sh

**To set up the Elastic Kubernetes Cluster (EKS) using the AWS console**, follow the following steps:

This is done by creating a jenkins pipeline that works on the Jenkinsfile and Jenkins-cluster file to create the eks cluster and also monitor it using proethues. Tis article <a href="https://www.jenkins.io/doc/tutorials/using-jenkinsfile-runner-github-action-to-build-jenkins-pipeline"/>gives an insight to getting this done</a?

**Destroying the resources**

Run **terraform destroy all**
