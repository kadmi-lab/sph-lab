# Test Lab for SPH Engineering

This project sets up a monitoring stack using Docker Compose, including the following services:
- **http-echo**: Simple HTTP server for testing.
- **Grafana**: Metrics vizualization
- **Prometheus**: Systems and service monitoring system.
- **Node Exporter**: Collects hardware and OS metrics
- **cAdvisor**: Containers monitoring
- **Blackbox Exporter**: Probes endpoints over HTTP

## Task Prerequisites

- **OS** - Ubuntu 22.04

- **Docker** >= 26.0.0: [Docker installation](https://docs.docker.com/engine/install/ubuntu/)
- **Docker Compose** >= 2.26.0: [Docker Compose installation](https://docs.docker.com/compose/install/linux/)

## Project tree

sph-lab/

├── docker-compose.yml

├── grafana/

│ └── provisioning/

├── prometheus/

│ └── prometheus.yml

└── blackbox/

│ └── blackbox.yml


## Running the Project

1. Clone the repository:

git clone https://github.com/kadmi-lab/sph-lab.git

2. Start the services:

docker compose up -d

3. Verify that the services are running:

docker ps

4. Accessing the Services via web

 http://-server-IP-:-defined-port-
 
 (Login into Grafana use default login and pass: admin/admin)

