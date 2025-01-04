# Infrastructure Monitoring Project

## Features
- **Ansible**: Automates the setup of Nginx and Grafana.
- **Docker**: Containers for Grafana and Prometheus.
- **GitLab CI/CD**: Automated build and deployment pipeline.
- **Kubernetes**: Orchestrates containers.

## Usage
1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```
2. Run Ansible playbook:
   ```bash
   ansible-playbook -i ansible/inventory/hosts ansible/playbooks/setup_nginx.yml
   ```
3. Start Docker services:
   ```bash
   docker-compose -f docker/docker-compose.yml up -d
   ```
