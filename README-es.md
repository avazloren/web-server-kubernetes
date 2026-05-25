# NGINX WEB SERVER ON KUBERNETES

![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

## ℹ️ Descripción

Archivos `yaml` para crear un `deployment` con 3 `réplicas` de un pod con un servidor web `nginx` en un clúster de `Kubernetes`.

El servicio que lo expone hacia el exterior del clúster es un `NodePort`.

<img width="614" height="138" alt="image" src="https://github.com/user-attachments/assets/25795c2e-c619-4966-b19a-b658aac756d1" />

## 🖥️ How to run it

```
kubectl apply -f .
kubectl port-forward svc/nginx-service 8080:80
curl localhost:8080
```
