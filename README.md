# 🚀 CI/CD Pipeline with GitHub Actions & Docker (No Cloud)

This project demonstrates a complete CI/CD pipeline using **GitHub Actions**, **Docker**, and **Docker Hub**, with **local deployment** via **Minikube (Kubernetes)** — no cloud provider required.

![ci-cd-banner](https://user-images.githubusercontent.com/placeholder/banner.png) <!-- Replace with real image if available -->

---

## 📌 Project Overview

- 🛠️ **Build**: A simple Python Flask app
- ✅ **Test**: Run unit tests using `pytest`
- 🐳 **Containerize**: Build Docker image
- 📤 **Publish**: Push image to Docker Hub
- 🚀 **Deploy**: Use Kubernetes (Minikube) to deploy locally

---

## 🧰 Tools & Technologies

| Tool         | Purpose                      |
|--------------|-------------------------------|
| GitHub Actions | CI/CD Workflow Automation     |
| Docker       | Containerization               |
| Docker Hub   | Image Registry                 |
| Flask        | Web Application Framework      |
| Pytest       | Python Unit Testing            |
| Minikube     | Local Kubernetes Cluster       |
| Kubernetes   | Deployment & Service Management|

---

## 📁 Project Structure


ci-cd-docker-pipeline/
├── .github/workflows/ci-cd.yml # GitHub Actions workflow
├── app/
│ ├── main.py # Flask app
│ ├── test_main.py # Unit test
│ └── requirements.txt # Flask + Pytest
├── Dockerfile # Docker build definition
├── k8s
   ├── deployment.yaml # Kubernetes Deployment
   ├── service.yaml # Kubernetes Service
└── README.md # Project documentation



---

## ⚙️ GitHub Actions Workflow

The pipeline automatically triggers on every push to the `main` branch:
1. Checkout code
2. Set up Python environment
3. Install dependencies and run tests
4. Build Docker image
5. Push image to Docker Hub

```yaml
trigger: [push → main]





🌐 Deployment On AWS EC2 (Minikube)

🚀 Step 1: Install kubectl (Kubernetes CLI)



🚀 Step 2: Install Minikube


🚀 Step 3: Install Docker (for Minikube driver)


🚀 Step 4: Start Minikube with Docker driver
    minikube start --driver=docker --force


## Apply Kubernetes Configs
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml


. Access the App

minikube service flask-service
# or visit http://localhost:30036













