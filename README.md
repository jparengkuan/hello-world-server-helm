# hello-world-server

A simple Node.js server deployed on Kubernetes, managed via ArgoCD.

## Features

- Node.js server application
- Kubernetes manifests for deployment and service
- GitOps workflow using ArgoCD

## Project Structure

- `hello-world-server/deployment.yaml`: Kubernetes Deployment manifest
- `hello-world-server/service.yaml`: Kubernetes Service manifest
- `application.yaml`: ArgoCD Application manifest

## Deployment

1. **Push manifests to GitHub**  
   Ensure all Kubernetes and ArgoCD manifests are committed and pushed.

2. **Set up ArgoCD**  
   Install ArgoCD on your Kubernetes cluster.

3. **Apply the ArgoCD Application**
   ```sh
   kubectl apply -f application.yaml