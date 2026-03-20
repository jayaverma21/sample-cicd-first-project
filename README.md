# Flask Azure App Service Deployment with Azure DevOps

This project demonstrates how to deploy a Flask web application to code base Azure App Service using an Azure DevOps YAML pipeline. The pipeline automates the process of installing dependencies, packaging the application, and preparing it for deployment using a ZIP-based approach. This showcases a simple and effective CI/CD workflow for Python web applications without using containers.

---

# Features
+ Flask Web Application: Lightweight Python web framework for building the app.
+ Azure DevOps CI/CD: Automates build and deployment using YAML pipeline.
+ ZIP-Based Deployment: Packages the application into a ZIP file for deployment.
+ Automated Dependency Installation: Installs required Python packages during pipeline execution.
+ Cloud Deployment: Deploys application to Azure App Service.
+ Simple Architecture: No Docker or containerization required.

---

# Requirements
+ Python 3.x  
+ Flask  
+ Azure DevOps account  
+ Azure Subscription  
+ Azure App Service  

---

# Installation
```bash
pip install -r requirements.txt

# Pipeline Explanation
+ The Azure DevOps pipeline (azure-pipelines.yml) performs the following steps:
+ Setsup Python Environment: Uses a specified Python version on the build agent.
+ Installs Dependencies: Creates a virtual environment and installs required packages.
+ Archives Application: Compresses the project files into a ZIP file.
+ Publishes Artifact: Stores the ZIP file as a build artifact for deployment.

# Deployment Type

+ Code-Based Deployment: Uses ZIP package deployment to Azure App Service.
+ Not Container-Based: No Docker image or container is used in this project.
