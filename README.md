# 🎬 Netflix Clone - DevSecOps Cloud Project

This project demonstrates a fully integrated **DevSecOps pipeline** to build, secure, deploy, and monitor a Netflix clone application on **AWS EC2 and Kubernetes**. It combines the power of **CI/CD, Container Security, GitOps, and Observability**, showing how a modern software delivery pipeline should function in production

<p align="center">
  <img width="1101" height="696" alt="Screenshot 2025-08-03 at 4 06 46 PM" src="https://github.com/user-attachments/assets/c7e7c1f9-f0e4-44e7-95df-88c0c2b44c95" />

</p>

🎥 **[Demo Video on YouTube](https://www.youtube.com/watch?v=YOUR_DEMO_LINK)**

---

## 🧠 What I Built

This project showcases how to build a production-grade, cloud-native Netflix clone using DevSecOps principles. I handled everything from provisioning infrastructure to deploying containers, securing the codebase, enabling automated CI/CD, implementing monitoring, and achieving GitOps delivery.  

This was not just a deployment task — it reflects:
- **Cloud knowledge (AWS EC2, Kubernetes, Helm)**
- **Security-first engineering (SonarQube, Trivy, OWASP scans)**
- **Infrastructure automation (Jenkins pipeline scripting, Docker image handling)**
- **Observability (Prometheus + Grafana dashboards, alert readiness)**
- **GitOps (ArgoCD syncing deployments from GitHub)**

---

## 🛠️ Tools & Technologies

| Domain            | Tools Used                                                                 |
|------------------|------------------------------------------------------------------------------|
| **Cloud & Infra** | AWS EC2, Ubuntu 22.04, Kubernetes (EKS/local), Helm                        |
| **CI/CD**         | Jenkins (Declarative Pipeline), GitHub, DockerHub                          |
| **Security**      | SonarQube (SAST), Trivy (Image scanning), OWASP Dependency-Check           |
| **Containerization** | Docker (Build, Tag, Push)                                               |
| **Deployment**    | Helm Charts, ArgoCD (GitOps sync to K8s)                                   |
| **Monitoring**    | Prometheus, Node Exporter, Grafana (dashboards, alerts)                    |
| **Notifications** | Jenkins Email Extension Plugin (email alerts for pipeline outcomes)        |

---

## 📊 DevSecOps Architecture

<p align="center">
  <img src="./assets/devsecops-architecture.png" alt="DevSecOps Architecture" width="800"/>
</p>

**Breakdown**:
- Jenkins pulls source code from GitHub and triggers a full CI/CD flow.
- Code quality and security is scanned with SonarQube and OWASP tools.
- Docker images are built, scanned with Trivy, and pushed to DockerHub.
- Helm deploys the app to a Kubernetes cluster.
- ArgoCD automatically syncs GitHub state to live K8s deployment.
- Prometheus + Grafana monitor metrics and display real-time dashboards.

---

## 🔍 Key Features & Skills Demonstrated

### ✅ CI/CD Pipeline (Jenkins)
- Multi-stage declarative pipeline using `Jenkinsfile`
- Integrates GitHub repo + Docker build + DockerHub push
- Static and dynamic security scanning embedded
- Pipeline breaks on failed quality gates or vulnerability reports

### ✅ Security Integration
- **SonarQube**: For static code analysis and maintainability checks
- **Trivy**: Docker image scanning for known vulnerabilities
- **OWASP Dependency-Check**: Node.js vulnerability scanning
- Breaks the pipeline if vulnerabilities are detected

### ✅ GitOps with ArgoCD
- Auto-sync Kubernetes deployments from GitHub using ArgoCD
- Source of truth maintained in version control
- Easy rollback and re-deploy from Git interface

### ✅ Kubernetes Deployment
- Dockerized app deployed via Helm chart
- Configured NodePort and service monitoring
- Full deployment lifecycle visible in ArgoCD UI

### ✅ Monitoring & Observability
- Node Exporter + Prometheus collect system and container metrics
- Grafana visualizes Jenkins metrics, app usage, and system health
- Configurable dashboards + alerting support

### ✅ Cloud Infrastructure
- EC2 instance hosting all components in a secured environment
- Custom security groups, firewall rules, and port exposures
- Cost-effective single-node demonstration setup

---

## 📸 Screenshots

### Jenkins CI/CD View
<img width="1305" height="157" alt="Screenshot 2025-08-03 at 6 53 51 PM" src="https://github.com/user-attachments/assets/45b905b7-ceb1-4772-bd11-c3fe71342c46" />

### Grafana Dashboard
<img width="1512" height="777" alt="Screenshot 2025-08-03 at 6 59 42 PM" src="https://github.com/user-attachments/assets/759681b8-3a94-47cc-b0b7-6e77de2353f7" />
<img width="1511" height="861" alt="Screenshot 2025-08-03 at 6 59 53 PM" src="https://github.com/user-attachments/assets/bce91448-ebd6-4329-9c6f-d00bfdcefc5d" />



### ArgoCD Sync

---

## 📁 Repository Structure

```
Netflix-DevOps/
├── Jenkinsfile                # Declarative CI/CD pipeline
├── Dockerfile                # Builds the Netflix clone app
├── charts/                   # Helm chart for K8s deployment
│   └── netflix/
├── assets/                   # Images for architecture, screenshots
├── dashboards/               # Grafana JSON files
├── scripts/                  # Setup scripts for Prometheus/Grafana
└── README.md
```

---

## 🙋‍♂️ About Me

Developed and maintained by [**Dhrumit Savaliya**](https://github.com/Dhrumit26) , [**Smit Lila**](https://github.com/Smitlila) 
🔗 Connect on [LinkedIn](https://www.linkedin.com/in/dhrumitvekariya)  
🛠 Passionate about DevOps | Cloud | Automation | CI/CD | Kubernetes

---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE)
