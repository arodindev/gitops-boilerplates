# ArgoCD Sample

Deploys [todoapp](https://github.com/arodindev/todoapp) and ArgoCD (for self sync).

Repo: https://github.com/arodindev/devops-boilerplates/tree/main/kubernetes

## Install ArgoCD on Cluster

```bash
kubectl apply -k https://github.com/arodindev/devops-boilerplates/kubernetes/argocd
```

## Install Istio on Cluster

```bash
istioctl install
```

## Apply `root` App

```bash
kubectl apply -k .
```

## Access ArgoCD Dashboard

Username: `admin`
Password: `kubectl get secrets -n argocd argocd-initial-admin-secret -o yaml`