# Sneakers E-commerce App with Complete DevOps Pipeline

This repository contains a React-based Sneakers e-commerce application enhanced with a full end-to-end DevOps pipeline and production-grade deployment using Jenkins, Docker, SonarQube, Trivy, Kubernetes (EKS), and Argo CD.

---

## About

This project started as a React-based Sneakers e-commerce app and enhanced the project by creating a complete DevOps pipeline and deployment setup from scratch, transforming it into a fully automated, secure, and production-ready cloud-native application.

---

## Key Features & Enhancements

- **Continuous Integration and Delivery (CI/CD) with Jenkins**  
  Automated build, test, and deployment triggered on every code push to GitHub.

- **Containerization with Docker**  
  Created Docker images of the React app for consistent runtime environments across development, testing, and production.

- **Code Quality & Security Scanning**  
  - **SonarQube** integration for continuous static code analysis and quality checks.  
  - **Trivy** vulnerability scanning for Docker images to detect security risks early.

- **Kubernetes Deployment on Amazon EKS**  
  Configured Kubernetes manifests (Deployment, Service) to run the app on a scalable and highly available Kubernetes cluster managed by EKS.

- **GitOps Deployment with Argo CD**  
  Declarative, automated continuous deployment using Argo CD, syncing Kubernetes cluster state with Git repository.

- **End-to-End Automation**  
  Entire pipeline from GitHub commits → Jenkins CI → Docker build → Quality & security scans → Docker Hub push → Argo CD deployment.

---

## Architecture Diagram

```plaintext
GitHub Repo
    ↓
Jenkins CI Pipeline
    ↓
Clone Code
    ↓
SonarQube Code Analysis & Quality Gate
    ↓
Build Docker Image
    ↓
Trivy Vulnerability Scan
    ↓
Push Docker Image to Docker Hub
    ↓
Argo CD Sync (Automated Deployment)
    ↓
Deploy to Kubernetes (EKS)
