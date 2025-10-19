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



<img width="1913" height="859" alt="image" src="https://github.com/user-attachments/assets/23bfb778-3252-4e89-881b-b18cf95c868c" />
<img width="1913" height="859" alt="image" src="https://github.com/user-attachments/assets/3cc20f51-9e3f-48f8-ac77-9b02f5abdfe8" />
<img width="1757" height="851" alt="image" src="https://github.com/user-attachments/assets/b348b7f8-4df2-444d-a601-e07c9a9a9a20" />

