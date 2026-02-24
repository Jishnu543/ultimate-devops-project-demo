# Microservices Infrastructure Implementation Lab
**Lead Engineer:** Jishnu Jayachandran
**Status:** Implementation Complete / Resources Decommissioned

## 📝 Project Objective
The goal of this project was to deploy and manage a high-scale microservices environment. I used this lab to master the interaction between polyglot services and to practice the full DevOps lifecycle—from initial containerization to final resource cleanup.

## 🛠️ My Technical Implementation
I followed a strict workflow to ensure the stability of the 11 microservices:
* **Container Strategy:** Verified Dockerfile efficiency for services in Python, Go, and Rust.
* **Orchestration:** Managed the cluster using Kubernetes manifests, focusing on Service discovery and Ingress routing.
* **Communication:** Validated gRPC connectivity between the frontend and back-end services.
* **Asynchronous Flow:** Observed Kafka message passing during the checkout-to-accounting pipeline.



## 📊 Observability & Validation
Before decommissioning the project, I implemented a monitoring stack to observe the "Golden Signals":
1. **Prometheus:** Configured to scrape metrics from the application pods.
2. **Grafana:** Built dashboards to visualize real-time traffic and error rates.
3. **OpenTelemetry:** Used for distributed tracing to find bottlenecks in service calls.



## 🧹 Cost Optimization & Resource Hygiene
A critical part of my DevOps practice is resource management. After validating the deployment:
* I performed a **full teardown** of the EKS/K8s cluster and associated Load Balancers.
* I used automated scripts (`cleanup_devops.py`) to ensure no orphan volumes or hidden costs remained.
* **Result:** 100% successful deployment with zero ongoing cloud expenditure.

---
**Technical Skills Demonstrated:** Kubernetes, Docker, Python Automation, SRE Observability, Cloud Cost Management.
