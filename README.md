# Despliegue de un Proyecto Django en Kubernetes con Minikube

Este documento detalla cómo desplegar un proyecto Django en Kubernetes utilizando Minikube.

## Prerrequisitos

Antes de comenzar, asegúrate de tener instalados los siguientes componentes:

- Docker
- Minikube
- Kubectl

## 4. Construir y Publicar la Imagen Docker

```bash
docker build -t your-docker-username/django-app:latest .
```

## 5. Desplegar en Kubernetes usando Minikube
```bash
minikube start
```

## 6. Aplicar Archivos YAML
```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

## 7.  Verificar la URL del Servicio
```bash
minikube service nombre-del-servicio --url
```