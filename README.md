# 🚀 End-to-End DevOps CI/CD Pipeline Project

## 📌 Project Overview

This project demonstrates a complete **CI/CD pipeline** built using modern DevOps tools.
It automates the process of **building, containerizing, and deploying an application to Kubernetes**.

---

## 🏗️ Architecture

```
GitHub → Jenkins → Docker → DockerHub → Kubernetes (Minikube)
```

---

## ⚙️ Tech Stack

* Version Control: Git & GitHub
* CI/CD Tool: Jenkins
* Containerization: Docker
* Container Registry: DockerHub
* Orchestration: Kubernetes (Minikube)
* Language: Python (Flask)

---

## 🔄 CI/CD Pipeline Flow

1. **Code Push**

   * Developer pushes code to GitHub repository

2. **Build Trigger**

   * Jenkins pipeline is triggered automatically

3. **Build Stage**

   * Docker image is built using Dockerfile

4. **Push Stage**

   * Image is pushed to DockerHub

5. **Deploy Stage**

   * Application is deployed to Kubernetes cluster

---

## 📂 Project Structure

```
.
├── app.py
├── requirements.txt
├── Dockerfile
├── Jenkinsfile
└── k8s/
    ├── deployment.yaml
    └── service.yaml
```

---

## 🐳 Docker Setup

### Build Image

```
docker build -t <dockerhub-username>/devops-pipeline-app .
```

### Run Container

```
docker run -d -p 5000:5000 <dockerhub-username>/devops-pipeline-app
```

---

## ☸️ Kubernetes Deployment

### Apply Deployment

```
kubectl apply -f k8s/deployment.yaml
```

### Apply Service

```
kubectl apply -f k8s/service.yaml
```

### Access Application

```
minikube service devops-service
```

---

## 🔐 Jenkins Configuration

* Added DockerHub credentials in Jenkins
* Configured pipeline using Jenkinsfile
* Enabled Docker and Kubernetes integration

---

## 🧪 Verification

```
kubectl get pods
kubectl get svc
```

---

## 📸 Screenshots 

<img width="1138" height="642" alt="Screenshot 2026-05-05 165058" src="https://github.com/user-attachments/assets/dd1e23c5-0152-431e-ac65-7c59f22f17df" />
<img width="1049" height="643" alt="Screenshot 2026-05-05 165047" src="https://github.com/user-attachments/assets/a4197e97-dda4-4370-9b8c-0ce8fb38b6d6" />
<img width="1213" height="948" alt="Screenshot 2026-05-05 163833" src="https://github.com/user-attachments/assets/8d6d8801-d938-46c8-bd8f-da3c402ec01f" />
<img width="1311" height="727" alt="Screenshot 2026-05-05 160959" src="https://github.com/user-attachments/assets/9d312d9a-c914-4882-a038-230398062389" />
<img width="1647" height="948" alt="Screenshot 2026-05-05 155556" src="https://github.com/user-attachments/assets/feceac42-a52e-413f-bf28-dfc9ddb4a833" />
<img width="1299" height="1066" alt="Screenshot 2026-05-05 150550" src="https://github.com/user-attachments/assets/067f23f8-e891-41ab-b502-689e89b2e414" />
<img width="1238" height="713" alt="Screenshot 2026-05-05 150520" src="https://github.com/user-attachments/assets/1ad7cd3b-b04f-45c5-ab9c-95e88fc2794e" />
<img width="1392" height="734" alt="Screenshot 2026-05-05 150354" src="https://github.com/user-attachments/assets/9ff096f8-5323-492a-94d4-95c7f6b43ab1" />
<img width="883" height="542" alt="Screenshot 2026-05-05 150040" src="https://github.com/user-attachments/assets/d8508f08-90bd-4057-987e-b591db282127" />
<img width="1399" height="906" alt="Screenshot 2026-05-05 150016" src="https://github.com/user-attachments/assets/672b4f68-9dee-4d85-a103-04cfe1073cce" />
<img width="314" height="319" alt="Screenshot 2026-05-05 145958" src="https://github.com/user-attachments/assets/3f5ba181-5ca2-445e-9571-83d4cfabb4aa" />
<img width="1920" height="1200" alt="Screenshot 2026-05-04 163335" src="https://github.com/user-attachments/assets/1c5916c6-ed8f-4ffc-9671-caea69470ea0" />


---

## 💡 Key Learnings

* Built complete CI/CD pipeline from scratch
* Solved real-world issues like:

  * Docker permission errors
  * Jenkins container networking
  * Kubernetes kubeconfig setup
* Integrated multiple DevOps tools seamlessly

---

## 🚀 Future Improvements

* Add Helm charts
* Implement monitoring (Prometheus + Grafana)
* Add automated testing stage
* Use cloud Kubernetes (EKS/GKE/AKS)

---

## 👩‍💻 Author

**Garima Kanwar**
DevOps / Cloud Enthusiast

---
