# django-todo-cicd

A DevOps project where I take an existing Django todo app and build the deployment side around it. The application itself is a standard Django todo (credit to the original author below); the containerization, Kubernetes manifests, and CI/CD setup are mine.

## What I added

- A Dockerfile that packages the app and its Python requirements into an image.
- A docker-compose.yml to run the app and its dependencies together.
- Kubernetes manifests under k8s/, including Secrets, to run the app on a cluster.
- A .dockerignore to keep the image lean.

The point of this repo is the deployment workflow, not the app: building the image, handling config and secrets, and getting a real application running on Kubernetes through a CI/CD pipeline.

## Credit

The base Django todo application is by Shrey Shah (shreys7/django-todo). This repo adds the Docker and Kubernetes deployment on top of it.
