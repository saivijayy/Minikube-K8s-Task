# 🚀 DevOps Internship - Task 5: Kubernetes with Minikube

## 🎯 Objective
Deploy and manage a sample application on a **local Kubernetes cluster** using **Minikube**.

---

## 🧰 Tools Used

- Minikube
- kubectl
- Docker
- YAML

---

## 📦 What Was Done

| Step | Description |
|------|-------------|
| ✅ | Installed Minikube and started the local Kubernetes cluster |
| ✅ | Created `deployment.yaml` for an Nginx deployment |
| ✅ | Created `service.yaml` to expose the app using NodePort |
| ✅ | Verified pods and services using `kubectl get pods` and `kubectl get svc` |
| ✅ | Scaled the deployment to 4 replicas |
| ✅ | Accessed the Nginx app in the browser via the Minikube service URL |

---

## 📂 Files

- `deployment.yaml` – Nginx deployment with initial 2 replicas
- `service.yaml` – NodePort service to expose Nginx app

---

## 🖼️ Screenshots

Screenshots included in the `screenshots/` folder:

- Pods before and after scaling
- Services output
- Browser access to Nginx

---

## 🔧 How to Use

### 1. Start Minikube
```bash
minikube start
```
### 2. Apply the Deployment
```bash
kubectl apply -f deployment.yaml
```
### 3. Apply the Service
```bash
kubectl apply -f service.yaml
```
### 4. View Pods and Services
```bash
kubectl get pods
kubectl get svc
```
### 5. Scale the Deployment  
```bash
kubectl scale deployment nginx-deployment --replicas=4
```
### 6. Access the App
```bash
minikube service nginx-service
```
