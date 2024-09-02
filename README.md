# E-Commerce Application Deployment

## Project Overview

This project deploys a simulated e-commerce application using Kubernetes. The application includes:
- **Frontend**: Served by Nginx, running a React-based web application.
- **Backend**: Node.js microservices handling various business operations.
- **Database**: MongoDB cluster for data persistence.
- **Message Queue**: RabbitMQ for asynchronous order processing.

## Deployment Instructions

### 1. Clone the Repository

cd k8s-ecommerce-deployment

### 2. Apply the Kubernetes Manifests
bash
Copy code
kubectl apply -f frontend.yaml
kubectl apply -f backend.yaml
kubectl apply -f mongodb.yaml
kubectl apply -f rabbitmq.yaml


### 3. Verify the Deployment
Check the status of the pods:
bash
Copy code
kubectl get pods
Ensure services are running:
bash
Copy code
kubectl get svc

### 4. Access the Application
Ensure that the frontend is accessible via the Ingress URL frontend.example.com.
