This project implements a DevSecOps pipeline to deploy a Netflix-style web application. The process includes automation, containerization, security scanning, and monitoring. Whenever code is pushed to the repository, the CI/CD pipeline automatically builds, scans, deploys, and monitors the application.

The workflow follows these stages:

Code Commit (GitHub)

Code is pushed to the repository, triggering the pipeline.

CI/CD Automation (Jenkins)

Jenkins pulls the code, installs dependencies, and initiates the build process.

Security Scanning (DevSecOps Stage)

SonarQube performs code quality and bug analysis.

OWASP Dependency Check scans for package vulnerabilities.

Trivy scans the filesystem/docker image for security issues.

Containerization (Docker)

The application is built into a Docker image and tested locally.

Image Push (DockerHub)

Once the image passes scans, it is pushed to a Docker registry.

Deployment (EC2 / Kubernetes)

The application is deployed using Docker containers or Kubernetes workloads.

Monitoring & Observability (Prometheus + Grafana)

System metrics, logs, and performance data are captured and visualized in dashboards.


Version Control -	Git, GitHub
CI/CD -	Jenkins
Containerization -	Docker
Registry - DockerHub
Security Scanning -	SonarQube, Trivy, OWASP Dependency Scanner
Cloud / Hosting -	AWS EC2 (or Kubernetes cluster)
Monitoring -	Prometheus, Grafana
Application Stack -	React / Node.js / API (Netflix Clone UI)
