# How to start with minikube

## Step 1: Install minikube
Follow official documentation on https://minikube.sigs.k8s.io/docs/start/

## Step 2: Start minikube

```bash
minikube start
minikube addons enable ingress
minikube ip
```

## Step 3: Deploy application
```bash
kubectl apply -f demo
```

Open the IP you got from `minikube ip` in your browser and you should see a running application.

## Step 4: Cleanup
```bash
minikube delete
```