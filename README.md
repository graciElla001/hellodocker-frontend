# hellodocker-frontend

## Image Tagging Strategy

Docker images are tagged with:

- `latest`: represents the most recent successful build
- Git commit SHA: uniquely identifies each version of the application

The commit SHA is generated using:

git rev-parse --short HEAD

This allows traceability and easy rollback to previous versions.

## CI/CD Pipeline

This project uses GitHub Actions to:

- Checkout code on every push
- Run a basic test step
- Build Docker images
- Tag images with `latest` and commit SHA
- Push images to Docker Hub

## Dockerhub repo
https://hub.docker.com/repository/docker/ijeoma12345/hellodocker-frontend/general
