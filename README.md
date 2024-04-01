# Kubernetes Project README

This repository contains the Kubernetes configuration files and setup instructions for deploying the `k8s_project_new` service using Docker, Kubernetes, and Minikube. This service runs a Tomcat server and can be accessed on any port of your choice.

## Project Directory Structure

k8s_project_new

│ Dockerfile

│ LICENSE

│ README.txt

│ deployment-service.yaml

│ pom.xml

└─── src

│ 
  └─── main
  
└─── target

## Prerequisites

Before you begin, ensure you have the following installed:

- Docker

- Minikube
  
- Kubernetes
  
- Maven

## Setup Instructions

Follow these steps to deploy the `k8s_project_new` service locally using Minikube:

1. **Clone Repository**: Clone this repository to your local machine.

2. **Build WAR File**: Generate the WAR file for the service using Maven:
   
```bash
mvn clean package
```
    
3. **Build Docker Image**: Build the Docker image for the service using the following command:

```bash
docker build -t vanshik123docker/sample-webapp:latest .
```
   
4. **Deploy to Kubernetes**: Apply the Kubernetes deployment and service YAML files:

```bash
minikube start
```
   
8. **Access the Application**: Once deployed, access the application using Minikube:

This command will open the application in your default web browser.

```bash
minikube service sample-webapp-service```

## Customization

- **Port Configuration**: You can access the application on any port of your choice by modifying the `deployment-service.yaml` file.

## Directory Structure

- **`/yaml-files`**: Contains the Kubernetes YAML files for deployment and service configurations.
- **`/src`**: Contains the source code for the `k8s_project_new` service.
- **`Dockerfile`**: Specifies the instructions to build the Docker image.
- **`README.md`**: This file providing setup instructions and project overview.






