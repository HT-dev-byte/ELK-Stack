# ELK-Stack

This project sets up the full ELK Stack (Elasticsearch, Logstash, Kibana, Filebeat) on Kubernetes using Docker containers and `kubectl` manifests.

## 🔧 Stack Components
- **Elasticsearch** – Data indexing and search engine
- **Logstash** – Pipeline for transforming logs
- **Filebeat** – Lightweight log shipper
- **Kibana** – Visualization UI

## 🚀 Features
- Deployed entirely on Kubernetes
- Configured Persistent Volumes for data retention
- Port-forwarding setup for GUI access
- Custom Resource Definitions (CRDs) used for Elastic Operator
- Sample Filebeat configuration to ship logs

## ⚙️ How to Deploy

```bash
kubectl apply -f elasticsearch.yaml
kubectl apply -f kibana.yaml
kubectl apply -f logstash.yaml
kubectl apply -f filebeat.yaml
