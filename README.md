# CI/CD Final Project

**Course:** CI/CD Tools and Practices  
**Project:** Continuous Integration and Continuous Delivery using GitHub Actions, Tekton, and OpenShift

## Project Overview

This project builds an automated CI/CD pipeline for the sample Python application provided in the course lab. The pipeline checks code quality, runs unit tests, builds an application image, and deploys the application to the lab’s OpenShift cluster.

## Project Objectives

- Use GitHub Actions to automate linting and unit testing.
- Create Tekton tasks for linting, unit testing, and building an image.
- Create an OpenShift Pipeline that runs those tasks.
- Add a deployment step that deploys the application to the lab OpenShift cluster.

## Tools and Technologies

- Python
- GitHub Actions
- Tekton
- Red Hat OpenShift Pipelines
- Kubernetes and containers

## Pipeline Overview

### Continuous Integration

The GitHub Actions workflow runs linting and unit tests when code changes are pushed or a pull request is opened.

### Build and Deployment

The OpenShift Pipeline runs the Tekton tasks to lint the code, run unit tests, build the application image, and deploy the application to the lab cluster.

## Repository Structure

- `.github/workflows/` — GitHub Actions workflow definitions
- `.tekton/` — Tekton task and pipeline definitions
- `service/` — Python application code
- `tests/` — Unit tests
- `Dockerfile` — Application image build instructions

## Lab Setup

Run the setup script from the lab terminal:

```bash
bash bin/setup.sh
