# Simplified-CICD-GitOps-with-Jenkins-and-ArgoCD
  
[![AWS Badge](https://img.shields.io/badge/Amazon_AWS-FFA500.svg?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/)
[![GitHub Badge](https://img.shields.io/badge/GitHub-181717.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Docker Badge](https://img.shields.io/badge/Docker-2496ED.svg?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/) 
[![ArgoCD Badge](https://img.shields.io/badge/ArgoCD-222222.svg?style=for-the-badge&logo=argocd&logoColor=white)](https://argoproj.github.io/argo-cd/)
[![Jenkins Badge](https://img.shields.io/badge/Jenkins-D24939.svg?style=for-the-badge&logo=jenkins&logoColor=white)](https://www.jenkins.io/)
[![Kubernetes Badge](https://img.shields.io/badge/Kubernetes-326CE5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![SonarQube Badge](https://img.shields.io/badge/SonarQube-4E9BCD.svg?style=for-the-badge&logo=sonarqube&logoColor=white)](https://www.sonarqube.org/)
[![Maven Badge](https://img.shields.io/badge/Maven-C71A36.svg?style=for-the-badge&logo=apache-maven&logoColor=white)](https://maven.apache.org/)

![non](https://github.com/kiranbakale/Simplified-CICD-GitOps-with-Jenkins-and-ArgoCD/assets/46279617/0bfb78ce-28f4-49c6-b6f3-be300bddc9dc)


# Project Name: Continuous Deployment with GitOps

## Overview

This repository demonstrates a comprehensive Continuous Integration and Continuous Deployment (CI/CD) setup using popular DevOps tools, emphasizing a GitOps approach. The tech stack includes AWS, Kubernetes (K8s), ArgoCD, Jenkins, SonarQube, Maven, Docker, and DockerHub.

## Folder Structure

- **/spring-boot-app**: Contains the source code of the application.
- **/spring-boot-app-manifests**: Includes Kubernetes deployment manifest files.

## CI/CD Flow

1. **Developer's Commit**: Developers commit their code to the GitHub repository.
2. **Jenkins Pipeline Trigger**: A Jenkins CI/CD pipeline is triggered automatically through the GitHub webhook.
3. **Code Analysis with SonarQube**: The pipeline performs code analysis using SonarQube to ensure code quality.
4. **Maven Build**: Maven is utilized to download required packages, build the application, and generate artifacts.
5. **Docker Containerization**: The application is containerized using Docker, and the Docker image is built.
6. **DockerHub Push**: The Docker image is pushed to DockerHub, ensuring availability and versioning.
7. **ArgoCD Image Updater**: ArgoCD's image updater component updates the image name in the repository.
8. **ArgoCD Deployment**: ArgoCD, the continuous delivery tool, orchestrates changes in the Kubernetes deployment based on the new image.

If you are interested in deploying this setup, follow the detailed step-by-step guide in this
[![Medium article]([https://img.shields.io/badge/Maven-C71A36.svg?style=for-the-badge&logo=apache-maven&logoColor=white](https://medium.com/@kiranbakale9/simplified-ci-cd-gitops-with-jenkins-and-argocd-b76de1c80362))]
This repository serves as a blueprint for implementing a GitOps-centric CI/CD pipeline, promoting automation and efficiency in the software delivery process. Feel free to customize and extend it based on your specific project needs.
