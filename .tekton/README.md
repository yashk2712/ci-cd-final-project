# CI/CD Final Project: OpenShift & GitHub Actions Workflows

## Project Overview
This project contains the continuous integration and continuous delivery (CI/CD) pipelines, Tekton tasks, and GitHub Actions configurations created for the **CI/CD Tools and Practices Final Project**. 

The project demonstrates automated testing, building, and deployment workflows targeting an OpenShift Cluster using a microservice application architecture.

## Repository Contents
* `.github/workflows/` - GitHub Actions workflow definitions for continuous integration (linting, testing, dependencies).
* `tekton/` - Custom Tekton pipeline definitions, tasks, and triggers for containerized builds via Buildah.
* `deploy/` - OpenShift deployment, service, and persistent volume configurations (`oc-lab-pvc`).
* `service/` - Application source code and unit test suite.

## Pipeline Features
* **Automated Code Linting:** Static code analysis using `flake8`.
* **Unit Testing & Coverage:** Test execution using `nosetests` with code coverage reports.
* **Image Building:** Container image assembly via OpenShift Tekton tasks (`buildah`).
* **Automated Deployment:** Cluster deployment updates to manage the `cicd-app` deployment.
