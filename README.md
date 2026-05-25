# NGINX WEB SERVER ON KUBERNETES

![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

## ℹ️ Description

`Yaml` files to create a `deployment` with 3 `replicas` of an `nginx` web server pod within a `Kubernetes` cluster.

The service that exposes it outside the cluster is a `NodePort`.

## 🖥️ How to run it

```
kubectl apply -f .
kubectl port-forward svc/nginx-service 8080:80
curl localhost:8080
```
