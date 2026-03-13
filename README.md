📅 **Date:** 13 March 2026
⏰ **Time:** 21:20 IST

Below is the **complete `README.md` file in proper Markdown format** including:

* Clean **project structure**
* **Docker workflow**
* **Kubernetes (Minikube) deployment**
* **Architecture**
* **Professional GitHub formatting**

You can **copy and paste this entire file into your `README.md`**.

---

# FULL README.md

```markdown
# Full Stack Chat Application Deployment

A real-time **full-stack chat application** containerized using **Docker** and deployed on **Kubernetes (Minikube)**.  
This project demonstrates how containerized applications can be orchestrated using Kubernetes and exposed using Kubernetes services.

---

# Project Overview

This project focuses on deploying a **containerized chat application** using modern DevOps tools.

Key Highlights:

- Containerized application using **Docker**
- Deployed application on **Kubernetes cluster using Minikube**
- Created **Kubernetes deployments and services**
- Demonstrates **microservices style deployment workflow**
- Local Kubernetes orchestration for development

---

# Architecture

```

Developer → Docker Image → Kubernetes (Minikube Cluster) → Chat Application

```

---

# Tech Stack

## Frontend
- React.js

## Backend
- Node.js
- Express.js
- Socket.io

## DevOps
- Docker
- Kubernetes
- Minikube
- kubectl

---

# Project Structure

```

full-stack-chatapp
│
├── backend
│   ├── server.js
│   ├── package.json
│
├── frontend
│   ├── src
│   ├── public
│   ├── package.json
│
├── kubernetes
│   ├── deployment.yaml
│   ├── service.yaml
│
├── Dockerfile
├── package.json
└── README.md

```

---

# Clone the Repository

```

git clone [https://github.com/MrSiddu73/full-stack-chatapp.git](https://github.com/MrSiddu73/full-stack-chatapp.git)

cd full-stack-chatapp

```

---

# Docker Setup

## Build Docker Image

```

docker build -t chatapp .

```

## Run Container

```

docker run -d -p 3000:3000 chatapp

```

Access application:

```

[http://localhost:3000](http://localhost:3000)

```

---

# Kubernetes Deployment (Minikube)

## Start Minikube Cluster

```

minikube start

```

---

## Apply Kubernetes Manifests

```

kubectl apply -f kubernetes/deployment.yaml

kubectl apply -f kubernetes/service.yaml

```

---

## Verify Pods

```

kubectl get pods

```

---

## Verify Services

```

kubectl get svc

```

---

# Access Application

If using **NodePort service**:

```

minikube service chatapp-service

```

Or access manually:

```

http://<minikube-ip>:<node-port>

```

---

# Kubernetes Resources Used

This project uses the following Kubernetes resources:

- **Deployment**
- **Service (NodePort)**

Deployment ensures application scaling and availability.

Service exposes the application externally.

---

# Learning Outcomes

Through this project I learned:

- Containerizing applications using Docker
- Running Kubernetes clusters locally using Minikube
- Deploying applications using Kubernetes manifests
- Managing Kubernetes pods and services
- Debugging containerized applications

---

# Future Improvements

Planned enhancements for this project:

- CI/CD pipeline using Jenkins
- GitOps deployment using ArgoCD
- Security scanning using Trivy
- Monitoring using Prometheus and Grafana
- Cloud deployment on AWS EKS

---

# Author

**Siddu Nyamagoud**

GitHub  
https://github.com/MrSiddu73

LinkedIn  
https://linkedin.com

```

---