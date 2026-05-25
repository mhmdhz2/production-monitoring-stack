# Production-Style Monitoring Infrastructure Stack

## Overview

This project is a centralized monitoring infrastructure built to simulate a production-style observability environment.

The stack continuously monitors:

- Linux server health
- Docker containers
- CPU usage
- Memory usage
- System load
- Network activity
- Container performance
- Uptime and availability

Metrics are collected using Prometheus exporters and visualized through Grafana dashboards.

---

## Architecture

```
Linux Server
│
├── Node Exporter
│     └── System Metrics
│
├── cAdvisor
│     └── Container Metrics
│
└── Prometheus
      └── Collects + Stores Metrics
              │
              ▼
          Grafana
              │
              ▼
     Visualization Dashboards
```

---

## Technologies Used

- Linux
- Docker
- Docker Compose
- Prometheus
- Grafana
- Node Exporter
- cAdvisor

---

## Features

✔ Centralized monitoring

✔ Real-time infrastructure visibility

✔ Docker container analytics

✔ Resource usage tracking

✔ Professional dashboards

✔ Metrics aggregation

✔ Multi-service deployment

✔ Infrastructure as Code

---

## Project Structure

```plaintext
monitoring-stack/
│
├── docker-compose.yml
├── README.md
├── prometheus/
│     └── prometheus.yml
│
└── screenshots/
```

---

## Monitoring Workflow

1. Node Exporter exposes Linux metrics
2. cAdvisor exposes Docker metrics
3. Prometheus scrapes exporters
4. Prometheus stores time-series data
5. Grafana visualizes dashboards

---

## Screenshots

### Prometheus Targets

![Prometheus Targets](screenshots/prometheus-target-health.png)

---

### Linux Server Monitoring Dashboard

![Linux Monitoring](screenshots/live-system-monitoring-dashboard.png)

---

### Container Monitoring Dashboard

![Container Monitoring](screenshots/grafana-container-monitoring-dashboard.png)

---

### Monitoring Stack Deployment

![Deployment](screenshots/docker-stack-deployment.png)

---

### Docker Compose Configuration

![Compose](screenshots/docker-compose-monitoring-stack-config.png)

---

### Prometheus Scrape Configuration

![Prometheus Config](screenshots/prometheus-scrape-configuration.png)
---

## Outcome

Successfully deployed a production-style monitoring environment capable of collecting, storing, and visualizing infrastructure metrics through centralized dashboards.

---

## Author

Mohamad Hazimeh
