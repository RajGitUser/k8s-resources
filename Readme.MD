🧩 k8s-resources

A collection of Kubernetes resource manifests (YAML files) demonstrating common Kubernetes objects — perfect for learning, prototyping, and reference.

This repository includes examples such as Namespaces, Pods, Deployments, Services, Secrets, ConfigMaps, ReplicaSets, StatefulSets, and more. 
GitHub

📌 Table of Contents

About

Repository Structure

Usage

List of Resources

Prerequisites

Apply Manifests

Contributing

License

🧠 About

This repo contains example Kubernetes YAML files showcasing basic and intermediate Kubernetes resources. It’s designed for:

✔ Learning and hands-on practice
✔ Training environments
✔ Reference templates for Kubernetes objects

📁 Repository Structure
k8s-resources/
├── volumes/
├── 01-namespace.yaml
├── 02-pod.yaml
├── 03-multi-container.yaml
├── 04-labels.yaml
├── 05-annotations.yaml
├── 06-resources.yaml
├── 07-env.yaml
├── 08-configmap.yaml
├── 09-pod-config.yaml
├── 10-secrets.yaml
├── 11-pod-secret.yaml
├── 12-service.yaml
├── 13-pod-service.yaml
├── 14-service-np.yaml
├── 15-pod-service-np.yaml
├── 16-service-lb.yaml
├── 17-pod-service-lb.yaml
├── 18-replicaset.yaml
├── 19-deployment.yaml
├── 20-statefulset.yaml
└── ... more YAML examples
``` :contentReference[oaicite:2]{index=2}

---

## 🚀 Usage

Clone this repository:

```bash
git clone https://github.com/RajGitUser/k8s-resources.git
cd k8s-resources


Ensure you have access to a Kubernetes cluster and kubectl is configured.

📜 List of Resources
File	                                Description
01-namespace.yaml	                    Defines a Namespace
02-pod.yaml	                            Basic Pod example
03-multi-container.yaml	                Pod with multiple containers
04-labels.yaml	                        Example showing labels
05-annotations.yaml	                    Example showing annotations
06-resources.yaml	                    Resource limits & requests
07-env.yaml	                            Environment variables in pods
08-configmap.yaml	                    ConfigMap example
09-pod-config.yaml	                    Use of ConfigMaps in Pods
10-secrets.yaml	                        Secret definition
11-pod-secret.yaml	                    Consuming Secrets in a Pod
12-service.yaml	                        Basic Service
13-pod-service.yaml	                    Pod + Service combination
14-service-np.yaml	                    Service with NetworkPolicy
15-pod-service-np.yaml	                Pod + Service + NetworkPolicy
16-service-lb.yaml	                    LoadBalancer Service
17-pod-service-lb.yaml	                Pod + LB Service example
18-replicaset.yaml	                    ReplicaSet
19-deployment.yaml	                    Deployment
20-statefulset.yaml	                    StatefulSet

Note: You may add more manifests as needed for other resources (Ingress, DaemonSet, Jobs, CronJobs, etc.). 
GitHub

🧰 Prerequisites

Before applying manifests, make sure:

✔ You have a running Kubernetes cluster (Minikube, Kind, EKS/GKE/AKS, etc.)
✔ kubectl CLI is installed and configured
✔ You have appropriate permission to create resources in your cluster

📌 Apply Manifests

To apply a particular YAML file:

kubectl apply -f <yaml-file>.yaml


Example:

kubectl apply -f 19-deployment.yaml


To delete a resource:

kubectl delete -f <yaml-file>.yaml

🤝 Contributing

Contributions are welcome! Here’s how you can help:

Add more Kubernetes examples

Improve existing manifests

Add documentation for advanced resources

Add GitHub Actions for automation

Fork the repo

Create a feature branch

Open a Pull Request

📄 License

This repository does not currently specify a license — Consider adding one (e.g., MIT) to allow reuse.