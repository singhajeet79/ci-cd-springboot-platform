# 🚀 Enterprise CI/CD Pipeline for Spring Boot Microservice

This repository demonstrates a **production-grade CI/CD pipeline** for a Spring Boot application using:

* Jenkins (CI/CD orchestration)
* Docker (containerization)
* Kubernetes (deployment)
* Prometheus + Grafana (observability)

---

## 🧱 Architecture

```
Developer
   ↓
GitHub
   ↓
Jenkins Pipeline
   ↓
Docker Build & Push
   ↓
Container Registry
   ↓
Kubernetes Deployment
   ↓
Monitoring (Prometheus + Grafana)
```

---

## ⚙️ Tech Stack

* Java (Spring Boot)
* Gradle
* Docker
* Kubernetes
* Jenkins
* Prometheus & Grafana

---

## 📂 Repository Structure

```
app/                # Spring Boot application
ci/                 # Jenkins pipeline
deployments/        # Kubernetes manifests
docker-compose/     # Local development setup
docs/               # Architecture and pipeline docs
```

---

## 🔁 CI/CD Pipeline

Pipeline stages:

1. Checkout code
2. Build (Gradle)
3. Run tests
4. Build Docker image
5. Tag with version (`BUILD_NUMBER`)
6. Push to registry
7. Deploy to Kubernetes

---

## 📦 Artifact Versioning

Docker images are versioned using:

```
<repo>:<BUILD_NUMBER>
```

Example:

```
springboot-app:42
```

This ensures:

* traceability
* rollback capability
* deployment consistency

---

## ☸️ Kubernetes Deployment

Apply manifests:

```bash
kubectl apply -f deployments/base/
```

---

## 📊 Observability

* Health endpoint: `/actuator/health`
* Metrics endpoint: `/actuator/prometheus`

Integrates with:

* Prometheus (metrics scraping)
* Grafana (dashboards)

---

## 🐳 Local Development

```bash
docker-compose up
```

---

## 📌 Key Features

* Production-ready CI/CD pipeline
* Kubernetes-ready deployment
* Health checks and monitoring
* Artifact versioning strategy
* Clean modular repository structure

---

## 🚀 Future Enhancements

* GitOps with ArgoCD
* Helm charts for deployment
* Security scanning (Trivy, Snyk)
* Multi-environment deployments

---

## 📖 Author

Ajeet Singh — DevOps & Platform Engineering
## Originally forked, heavily refactored into production-grade system
