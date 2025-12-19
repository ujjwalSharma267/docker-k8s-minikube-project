# Docker + Kubernetes CI/CD Project (Minikube)

## Overview
End-to-end DevOps project demonstrating Docker containerization,
Kubernetes deployment using Minikube, and CI automation using GitHub Actions.

## Tech Stack
- Docker
- Kubernetes (Minikube)
- GitHub Actions
- Node.js
- Ubuntu (WSL)
- VS Code

## Architecture
GitHub → CI (Docker Build) → Local CD → Kubernetes Cluster

## How to Run Locally
```bash
minikube start --driver=docker
minikube image build -t docker-k8s-demo:1.0 app/
kubectl apply -f manifests/
minikube service demo-service
