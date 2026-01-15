# Voting App on Kubernetes

I worked on a multi-service Voting Application deployed on Kubernetes.
The application follows a microservices architecture where the Voting App frontend allows users to cast votes, which are temporarily stored in Redis acting as a cache and message queue.
A Worker App processes these votes asynchronously and stores the final data in PostgreSQL.
The Result App then fetches data from PostgreSQL to display live voting results.
Each component runs in its own Kubernetes Deployment and is exposed internally using Kubernetes Services for service discovery and communication.
Kubernetes ensures scalability, self-healing, and high availability.
For observability, I integrated Prometheus to collect cluster and application metrics and Grafana to visualize CPU, memory, pod health, and service performance.
This project demonstrates my hands-on experience with container orchestration, service management, monitoring, and troubleshooting in a real-world DevOps setup.

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

