# 🔍 DevOps System Monitor (Cloud + Container + Kubernetes)

<p align="center">
A Python-based system monitoring tool built and evolved into a full DevOps workflow — from local script to cloud deployment and Kubernetes orchestration.
</p>

---

## 📊 Project Status

<p align="center">

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Docker](https://img.shields.io/badge/Container-Docker-blue?logo=docker)
![AWS](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazonaws)
![Kubernetes](https://img.shields.io/badge/Orchestration-Kubernetes-blue?logo=kubernetes)
![Status](https://img.shields.io/badge/Status-Active-success)
![DevOps](https://img.shields.io/badge/Focus-DevOps%20Learning-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

</p>

---

## 🚀 Overview

This project started as a simple **Python CLI monitoring tool** and was progressively developed into a **cloud-native DevOps project**.

It now demonstrates a full workflow:

- Monitor system resources (CPU, Memory, Disk)
- Log and track system performance over time
- Containerize the application using Docker
- Deploy on a cloud server (AWS EC2)
- Store container images in AWS ECR
- Run workloads using Kubernetes

This mirrors how real-world systems are built and deployed in production environments.

---

## 🧠 Why I Built This

This is part of my **daily DevOps engineering challenge**, where I focus on building practical, real-world systems instead of just studying theory.

This project helped me understand:

- How monitoring works at a system level
- How applications are packaged using containers
- How cloud infrastructure runs workloads
- How Kubernetes manages and scales applications

---

## ⚙️ Tech Stack

- Python 3
- psutil
- Docker
- AWS EC2
- AWS ECR
- Kubernetes (Minikube)

---

## 🔧 Features

- Real-time system monitoring
- Continuous logging to file
- Threshold-based alerting
- Containerized application
- Cloud deployment on AWS
- Kubernetes-based orchestration

---

## 📦 Installation (Local)

```bash
git clone <your-repo-url>
cd devops-system-monitor
pip3 install -r requirements.txt
```

---

## ▶️ Run Locally

```bash
python3 monitor.py
```

---

## 🐳 Docker Setup

### Build Image

```bash
docker build -t system-monitor .
```

### Run Container

```bash
docker run system-monitor
```

---

## ☁️ AWS Deployment (EC2)

1. Launch EC2 instance
2. Connect via SSH
3. Install Python & Docker
4. Run the containerized application

---

## 📦 Push to AWS ECR

```bash
aws ecr create-repository --repository-name system-monitor

docker tag system-monitor:latest <ECR_URI>

docker push <ECR_URI>
```

---

## 🚀 Deploy from ECR

```bash
docker pull <ECR_URI>
docker run -d <ECR_URI>
```

---

## ☸️ Kubernetes Deployment

### Apply Deployment

```bash
kubectl apply -f deployment.yaml
```

### Check Running Pods

```bash
kubectl get pods
```

### View Logs

```bash
kubectl logs <pod-name>
```

---

## 🧱 Architecture

```
Local Machine
   ↓
Python Monitoring Script
   ↓
Docker Container
   ↓
AWS EC2 Instance
   ↓
AWS ECR (Image Registry)
   ↓
Kubernetes Cluster (Minikube)
```

---

## 📸 Demo

_Add screenshots here (recommended):_
- CLI output running
- Docker container running
- Kubernetes pods running

---

## 📈 What I Learned

- How system monitoring works in real environments
- How to containerize applications using Docker
- How AWS EC2 is used to run workloads
- How ECR stores and distributes container images
- How Kubernetes manages containerized applications
- How DevOps workflows connect everything together

---

## 🔥 Future Improvements

- Add Slack/email alerting system
- Store logs in a database
- Build a web-based monitoring dashboard
- Deploy fully on AWS EKS
- Add CI/CD pipeline with GitHub Actions

---

## 👨‍💻 Author

**Tristan Jones**  
Aspiring Cloud Engineer | AWS Certified  
