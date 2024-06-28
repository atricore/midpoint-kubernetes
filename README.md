# Midpoint Kubernetes

## Deployment

Use `kustomize` to deploy for your env:

```bash
kubectl apply -k ./envs/gke/
```

## Description

* envs: configuration specific for different k8s environments
* base: basic configuration
* config: midpoint configuration. You can add XML object configs
* secrets: used by DB and MD, you should patch them using **kustomize**
* midpoint: resources deploying midpoint server and repository
