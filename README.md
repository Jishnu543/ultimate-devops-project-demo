# Microservices Infrastructure Lab (DevOps Demo)
**Project Lead: Jishnu Jayachandran**

## 🚀 Project Overview
This is a comprehensive Microservices-based project designed to demonstrate production-grade DevOps practices. It features a polyglot architecture with services written in **Python, Go, Java, Node.js, C++, and Ruby**, utilizing **gRPC** for high-performance communication.

## 🏗️ System Architecture
The application is a web-based e-commerce platform consisting of the following core components:

| Service | Language | Description |
| :--- | :--- | :--- |
| **Frontend** | Next.js | User-facing web interface. |
| **Cart Service** | .NET | Manages user shopping carts. |
| **Product Catalog** | Go | Provides product metadata. |
| **Currency Service** | C++ | Handles real-time currency conversion. |
| **Payment Service** | Node.js | Processes secure transactions. |
| **Shipping Service** | Rust | Calculates shipping rates/tracking. |
| **Email Service** | Ruby | Sends order confirmations. |
| **Recommendation** | Python | Uses AI/ML logic for product suggestions. |

## 🛠️ DevOps & Infrastructure Stack
* **Containerization:** All services are Dockerized for consistency across environments.
* **Orchestration:** Includes production-ready **Kubernetes (K8s)** manifests.
* **CI/CD:** Integrated with GitHub Actions for automated testing and deployment.
* **Observability:** Full stack integration with **OpenTelemetry**, **Prometheus**, **Grafana**, and **Jaeger** for distributed tracing.
* **Messaging:** Uses **Kafka** for asynchronous communication between the checkout and accounting services.

## 🔧 Deployment Guide
### 1. Local Development (Docker Compose)
Run the entire stack locally with a single command:
```bash
docker-compose up -d
```

### 2. Kubernetes Deployment
Deploy to any K8s cluster (EKS, GKE, or Minikube):
```bash
kubectl apply -f ./kubernetes/complete-deploy.yaml
```

## 🧪 Custom Automation
I have added custom maintenance scripts to handle the infrastructure lifecycle:
* `health_check.py`: Validates service availability across the mesh.
* `cleanup_devops.py`: Automated cleanup of Docker and K8s resources.

---
*This project is maintained by Jishnu Jayachandran to showcase advanced skills in Cloud-Native Infrastructure and Site Reliability Engineering (SRE).*
