# Kubernetes-Compose
kompose is a tool to help users who are familiar with docker-compose move to Kubernetes. kompose takes a Docker Compose file and translates it into Kubernetes resources.

kompose is a convenience tool to go from local Docker development to managing your application with Kubernetes. Transformation of the Docker Compose format to Kubernetes resources manifest may not be exact, but it helps tremendously when first deploying an application on Kubernetes.

# Use Case
Convert docker-compose.yaml into Kubernetes deployments and services with one simple command:

$ kompose convert -f docker-compose.yaml
INFO Kubernetes file "frontend-service.yaml" created         
INFO Kubernetes file "redis-master-service.yaml" created     
INFO Kubernetes file "redis-slave-service.yaml" created      
INFO Kubernetes file "frontend-deployment.yaml" created      
INFO Kubernetes file "redis-master-deployment.yaml" created  
INFO Kubernetes file "redis-slave-deployment.yaml" created 

# Installation 
We have multiple ways to install Kompose. Our preferred method is downloading the binary from the latest GitHub release.
Our entire list of installation methods are located in our installation.md document.

# Installation methods:

Binary (Preferred method)
Go
CentOS
Fedora
openSUSE/SLE
macOS (Homebrew)
Windows

# 1. Binary installation
Kompose is released via GitHub on a three-week cycle, you can see all current releases on the GitHub release page.
Linux and macOS:

# 2. Linux
curl -L https://github.com/kubernetes/kompose/releases/download/v1.20.0/kompose-linux-amd64 -o kompose

# 3. macOS
curl -L https://github.com/kubernetes/kompose/releases/download/v1.20.0/kompose-darwin-amd64 -o kompose

chmod +x kompose
sudo mv ./kompose /usr/local/bin/kompose


Windows:

Download from GitHub and add the binary to your PATH.

Note: kompose up is not supported on windows.
