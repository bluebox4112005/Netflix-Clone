## 📌 How the Project Works

This project uses a complete **DevSecOps pipeline** to deploy a Netflix-style web application. The pipeline automates building, testing, securing, containerizing, deploying, and monitoring the application.

---

### 🔄 Workflow Overview

- **Code Commit (GitHub)**  
  Developer pushes code to GitHub which triggers the CI/CD pipeline.

- **CI/CD Automation (Jenkins)**  
  Jenkins pulls the code, installs dependencies, and starts the build process.

- **Security Scanning (DevSecOps Stage)**  
  - **SonarQube:** Code quality and vulnerability analysis  
  - **OWASP Dependency Check:** Library and package vulnerability scan  
  - **Trivy:** Filesystem and container security scanning

- **Containerization (Docker)**  
  The application is packaged into a Docker image and tested locally.

- **Image Push (DockerHub)**  
  Once validated, the image is pushed to DockerHub for deployment use.

- **Deployment (EC2 / Kubernetes / Container Runtime)**  
  The application is deployed in a cloud environment and made accessible.

- **Monitoring (Prometheus + Grafana)**  
  Metrics and logs are collected and visualized for health, performance, and alerts.

---

## 🛠️ Tools Used

| Stage | Tools |
|-------|--------|
| Version Control | Git, GitHub |
| CI/CD | Jenkins |
| Security Scanning | SonarQube, Trivy, OWASP Dependency-Check |
| Containerization | Docker |
| Registry | DockerHub |
| Deployment | AWS EC2 / Kubernetes |
| Monitoring | Prometheus, Grafana |

---
