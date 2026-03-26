# 🚀 CI/CD Spring Boot Platform

Production-grade DevOps pipeline demonstrating CI/CD + GitOps for a containerized Spring Boot service.

## 🧱 Architecture
GitHub → CI → Docker Hub → ArgoCD → Kubernetes

## ⚙️ Stack
Spring Boot (Java 17), Gradle, Docker, Kubernetes, ArgoCD, Prometheus, Grafana

## 🔁 Pipeline<img width="1917" height="953" alt="Screenshot from 2026-03-26 15-04-47" src="https://github.com/user-attachments/assets/df7efb12-783f-4606-b93a-8d171c6395ec" />

- Build & test
- Docker image (tagged with git SHA)
- Push to registry
- Auto-deploy via ArgoCD (GitOps)

## 📌 Highlights
- Immutable deployments
- GitOps-based delivery
- Kubernetes-ready setup
- Clean, modular structure

## 👤 Author
Ajeet Singh — AI/ML/DevOps / Platform Engineering
