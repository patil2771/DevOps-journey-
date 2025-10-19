# Voting App on Kubernetes

## Overview
This is a **multi-service Voting App** deployed on Kubernetes, demonstrating container orchestration, service management, and monitoring. The app includes the following components:  

- **PostgreSQL** – Database for storing votes  
- **Redis** – Caching and message queue  
- **Voting App** – Frontend for voting  
- **Worker App** – Background processing  
- **Result App** – Display voting results  

Monitoring and observability are implemented using **Prometheus and Grafana** to track application and cluster metrics.

---

## Repository Structure

voting-app/
├── README.md
├── postgres-deployment.yaml
├── postgres-pod.yaml
├── postgres-service.yaml
├── redis-deployment.yaml
├── redis-pod.yaml
├── redis-service.yaml
├── voting-app-deployment.yaml
├── voting-app-pod.yaml
├── voting-app-service.yaml
├── worker-app-deploy.yaml
├── worker-pod.yaml
├── result-app-deployment.yaml
├── result-app-pod.yaml
└── result-app-service.yaml
