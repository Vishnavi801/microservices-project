# Microservices Application Deployment on AWS EKS

## Project Overview

This project demonstrates the deployment of a cloud-native microservices application on Amazon EKS using Jenkins CI/CD pipelines and Kubernetes.

The application consists of multiple interconnected services that simulate a real-world e-commerce platform. Jenkins automates the deployment process by applying Kubernetes manifests to the EKS cluster.

## Technologies Used

* AWS EKS
* Kubernetes
* Jenkins
* Docker
* GitHub
* kubectl

## Microservices Included

* Frontend
* Product Catalog Service
* Cart Service
* Checkout Service
* Payment Service
* Recommendation Service
* Currency Service
* Shipping Service
* Email Service
* Ad Service
* Redis

## Architecture

Developer
→ GitHub Repository
→ Jenkins Pipeline
→ AWS EKS Cluster
→ Kubernetes Deployments
→ Kubernetes Services
→ End Users

## Kubernetes Resources Used

### Deployments

Used for managing application pods and ensuring high availability.

### Services

* ClusterIP
* NodePort
* LoadBalancer

### Health Checks

* Readiness Probe
* Liveness Probe

### Resource Management

* CPU Requests
* CPU Limits
* Memory Requests
* Memory Limits

## Jenkins Pipeline Workflow

1. Jenkins connects to AWS EKS using Kubernetes credentials.
2. Deployment manifests are applied to the cluster.
3. Kubernetes creates and manages the application pods.
4. Jenkins validates the deployment by verifying services.

## Commands Used

kubectl apply -f deployment-service.yml

kubectl get pods

kubectl get svc

kubectl get deployments

## Key Learnings

* Kubernetes application deployment
* AWS EKS cluster management
* Jenkins CI/CD integration
* Microservices architecture deployment
* Kubernetes networking concepts
* Health monitoring using readiness and liveness probes

## Outcome

Successfully deployed a multi-service application on AWS EKS using Jenkins automation and Kubernetes orchestration.
