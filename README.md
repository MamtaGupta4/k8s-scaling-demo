# 🚀 Kubernetes Scaling & Self-Healing Demo

This project demonstrates Kubernetes scaling and self-healing capabilities using an Nginx Deployment.

## 🛠 Technologies Used

- Kubernetes
- Minikube
- Docker
- Nginx
- kubectl

## 📂 Project Structure

```text
k8s-scaling-demo/
│
├── deployment.yaml
└── README.md
```

## 🚀 Deployment

Apply the deployment:

```bash
kubectl apply -f deployment.yaml
```

Check deployment and pods:

```bash
kubectl get deployments
kubectl get pods
```

## 📈 Scaling

Scale the deployment from 2 to 5 replicas:

```bash
kubectl scale deployment nginx-deployment --replicas=5
```

## 🔄 Self-Healing

Delete a running pod:

```bash
kubectl delete pod <pod-name>
```

Monitor pod recreation:

```bash
kubectl get pods -w
```

Kubernetes automatically creates a new pod to maintain the desired replica count.

## 🎯 Concepts Covered

- Deployment
- ReplicaSet
- Pods
- Scaling
- Self-Healing

## ✅ Result

Successfully deployed an Nginx application, scaled it to multiple replicas, and verified Kubernetes self-healing through automatic pod recreation.
