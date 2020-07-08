# Jaeger Elasticsearch Minikube setup

This repository creates a helm chart for Jaeger backed by Elasticsearch ready to be deployed on minikube cluster.

## Pre-requisites

- helm2, v2.16.9 (tested version)
- minikube, v1.11.0 (tested version)

## Environment setup instructions

Create a Minikube cluster using :

```bash
minikube start --vm-driver=virtualbox --cpus=4 --memory=4g
```

## Running instructions

Deploy this helm chart using using:

```bash
helm install --name release-name ./
```

> **Note:** Elasticsearch will take some time to spin up. Meanwhile, Jaeger collector, and Jaeger query will be breaking. Wait for 2 minutes to reflect the changes in Jaeegr chart :)

## Test setup

Follow the helm-chart notes to test the setup.
