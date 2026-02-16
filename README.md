🚀 Java Microservices Deployment on Kubernetes (Docker + Minikube on AWS EC2)

A hands-on DevOps project demonstrating an end-to-end deployment workflow for a Java microservices application using Maven, Docker, Docker Hub, and Kubernetes. The services are deployed on a Kubernetes cluster running on Minikube inside an AWS EC2 instance, using production-style Kubernetes Deployments and Services.


📌 Project Overview

This repository showcases a real DevOps deployment pipeline:
Java Microservices → Maven Build → JAR Packaging → Docker Image → Docker Hub → Kubernetes Deployments → Service Exposure
The goal of this project is to simulate how Java applications are built, containerized, published, and deployed in modern cloud-native environments.


🧩 Microservices Included

| Service              | Description                                    | Port |
| -------------------- | ---------------------------------------------- | ---- |
| **shopfront**        | Frontend service for accessing the application | 8010 |
| **productcatalogue** | Handles product catalogue APIs                 | 8020 |
| **stockmanager**     | Manages stock and availability APIs            | 8030 |


🏗️ Architecture (High Level)

Each microservice is packaged as a JAR
Each service runs as an independent Docker container
Images are stored in Docker Hub
Kubernetes manages:
Deployments (replicas + rolling updates)
Services (NodePort) for exposure inside Minikube


🛠️ Tech Stack

Java
Maven
Docker
Docker Hub
Kubernetes
Minikube
AWS EC2
Git & GitHub


📌 Kubernetes Manifests

The Kubernetes manifests include:
✅ Deployments (Pods, scaling, rolling updates)
✅ NodePort Services (exposure for testing)
✅ Reusable YAML structure for real deployment practice
All files are located inside the kubernetes/ directory.


🎯 What I Learned from This Project

Building Java microservices using Maven
Writing Dockerfiles for Java JAR-based applications
Publishing images to Docker Hub
Deploying applications to Kubernetes using YAML
Understanding Kubernetes Deployments vs Services
Exposing services using NodePort in Minikube
Running Kubernetes on an EC2 instance for hands-on practice


📌 Future Improvements (Planned)

Add Ingress for routing instead of NodePort
Add CI/CD pipeline (GitHub Actions / Jenkins)
Add monitoring using Prometheus + Grafana
Add Helm charts for easier deployments


📫 Connect With Me

LinkedIn: https://www.linkedin.com/in/madhusudhan-reddy-8143a5234
