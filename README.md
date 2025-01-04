# Infrastructure Monitoring Project
project/
├── ansible/
│   ├── inventory/
│   │   ├── hosts
│   ├── playbooks/
│   │   ├── setup_nginx.yml
│   │   ├── setup_grafana.yml
│   │   ├── deploy_monitoring.yml
├── docker/
│   ├── grafana/
│   │   ├── Dockerfile
│   │   ├── grafana.ini
│   ├── nginx/
│   │   ├── Dockerfile
│   │   ├── nginx.conf
├── kubernetes/
│   ├── deployments/
│   ├── services/
│   ├── ingress/
├── ci_cd/
│   ├── .gitlab-ci.yml
│   ├── Jenkinsfile (اختیاری)
├── README.md
├── scripts/
│   ├── setup.sh
│   ├── cleanup.sh
└── docs/
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
