# Voting App on Kubernetes

## Overview
Multi-service Voting App deployed on Kubernetes, including:
- PostgreSQL
- Redis
- Voting App
- Worker App
- Result App

Monitoring and observability implemented with Prometheus and Grafana.

## Deployment
1. Apply manifests in order:
   ```bash
   kubectl apply -f manifests/postgres/
   kubectl apply -f manifests/redis/
   kubectl apply -f manifests/voting-app/
   kubectl apply -f manifests/worker-app/
   kubectl apply -f manifests/result-app/
   kubectl apply -f manifests/monitoring/
