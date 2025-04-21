```markdown
# 🚀 MLOps-Kubernetes Project: Scalable Machine Learning Deployment

![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)

A hands-on project demonstrating **end-to-end MLOps workflows** with Kubernetes, Docker, and Flask. Designed to showcase expertise in containerization, orchestration, and scalable ML deployment.

## 📌 Project Overview
Deploy a machine learning application in a production-grade Kubernetes environment, featuring:
- **Containerization** with Docker
- **Orchestration** via Kubernetes
- **Load balancing** for high availability
- **Performance monitoring** with Minikube Dashboard

## 🛠️ Key Features
- **CI/CD Pipeline Integration**: From code to containerized deployment
- **Auto-Scaling**: Kubernetes-managed pods for dynamic workloads
- **Local Development**: Minikube-based Kubernetes cluster
- **Performance Testing**: Postman-driven load testing

## 🧩 Technologies Used
- **Containerization**: Docker
- **Orchestration**: Kubernetes, Minikube
- **Web Framework**: Flask (Python)
- **Monitoring**: Minikube Dashboard
- **Load Testing**: Postman

## 🛠️ Getting Started

### Prerequisites
- Docker Desktop
- Kubernetes (Minikube)
- Python 3.8+

```bash
# Clone repository
git clone https://github.com/Jittub45/MLOps-Kubernetes.git

# Install dependencies
pip install -r requirements.txt
```

### 🐳 Build & Run Locally
```bash
# Build Docker image
docker build -t kubernetes-test-app:latest .

# Run container
docker run -p 5000:5000 kubernetes-test-app:latest
```

## ☸️ Kubernetes Deployment
```bash
# Start Minikube cluster
minikube start --nodes=2 --embed-certs

# Load Docker image to Kubernetes
minikube image load kubernetes-test-app:latest

# Deploy application
kubectl apply -f deployment.yaml
```

### 🔍 Verify Deployment
```bash
kubectl get pods -A
kubectl get deployments
minikube service kubernetes-test-app
```

## 📊 Monitoring & Scaling
```bash
# Access Kubernetes dashboard
minikube dashboard

# Check pod logs
kubectl logs -f <pod-id>
```

## ⚖️ Load Testing
1. Open Postman
2. Create performance test with:
   - **10 Virtual Users**
   - **1 Minute Duration**
3. Analyze results through Kubernetes dashboard


## 📜 License
MIT License - See [LICENSE](LICENSE)

---

💡 **Why This Matters**  
This project demonstrates critical MLOps skills recruiters look for:
- Production-grade deployment strategies
- Container orchestration at scale
- Infrastructure-as-Code (IaC) through YAML
- Performance optimization insights

Perfect for roles requiring Kubernetes expertise in ML deployment pipelines!
```

