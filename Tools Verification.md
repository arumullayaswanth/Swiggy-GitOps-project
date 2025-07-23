
# ✅ Installation Verification Checklist

```bash
# Git
git --version
> ✅ Should show `active (running)`

# Java
java -version
> ✅ Should return output with `openjdk version "17..."`

# Jenkins
systemctl status jenkins
> ✅ Should show `active (running)`

# Terraform
terraform -v
> ✅ Should return `Terraform v1.x.x`

# Maven
mvn -v
> ✅ Should return `Apache Maven x.x.x`

# kubectl
kubectl version --client
> ✅ Should show `Client Version: v1.xx.x`

# eksctl
eksctl version
> ✅ Should show `eksctl version: x.x.x`

# Helm
helm version
> ✅ Should return something like `v3.6.x`

# Docker
docker --version
> ✅ Should return `Docker version xx.xx.xx`

docker ps
> ✅ Should list running containers like `sonarqube` or others

# Trivy
trivy --version
> ✅ Should return `Version: 0.48.3`

# MariaDB
mysql --version
> ✅ Should return something like `mysql  Ver x.x Distrib...`

systemctl status mariadb
> ✅ Should show `active (running)`

# ArgoCD
kubectl get pods -n argocd
> ✅ Should list ArgoCD pods, all in `Running` or `Completed` status

# Prometheus / Grafana
kubectl get pods -n prometheus
> ✅ Should list Prometheus and Grafana pods, all in `Running` or `Completed` status
```
```bash
DevOps-Environment/
├── Source Control
│   └── git
│
├── CI/CD
│   ├── jenkins
│   ├── maven
│   ├── docker
│   │   └── docker-compose
│   └── sonar (via Docker)
│
├── Infrastructure as Code (IaC)
│   ├── terraform
│   ├── awscli
│   ├── eksctl
│   ├── kubectl
│   └── helm
│
├── Kubernetes Tools
│   ├── argocd
│   ├── prometheus
│   ├── grafana
│   └── k9s
│
├── Security & Compliance
│   ├── trivy
│   └── vault (optional)
│
├── Databases
│   ├── mariadb
│   └── postgresql
│
├── Web Servers & Proxies
│   └── nginx (optional)
│
├── Programming Runtimes
│   ├── java-17 (for Jenkins)
│   ├── nodejs & npm (optional)
│   └── python3 & pip
│
├── Configuration Management
│   └── ansible
│
├── Monitoring & System Utilities
│   ├── htop
│   ├── net-tools
│   └── systemctl (for service checks)
│
└── Optional DevOps Tools
    ├── keycloak
    ├── harbor (private registry)
    └── gitlab (code hosting & CI/CD)
```
