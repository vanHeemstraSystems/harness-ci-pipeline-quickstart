# 100 - Harness Community Edition Deployment Tutorial

Based on "Harness Community Edition Deployment Tutorial" at https://docs.harness.io/article/ltvkgcwpum-harness-community-edition-quickstart

This quickstart shows you how to set up Harness CD Community Edition locally and create a CD Pipeline that deploys a public NGINX image to a local cluster.

Harness CD Community Edition is a lightweight version of Harness that you can download and run on your laptop or any VM with 3GB RAM and 2 CPUs. Harness CD Community Edition is intended to get devs started with Harness quickly without having to sign up for a Harness SaaS account.

**NOTE**: For an overview, see [Harness CD Community Edition Overview](https://docs.harness.io/article/yhyyq0v0y4-harness-community-edition-overview).

## 100 - Objectives

You'll learn how to:

- Install and run Harness CD Community Edition locally.
- Create and deploy a CD Pipeline in Harness CD Community Edition using a public Docker image and a local Kubernetes cluster.

## 200 - Requirements

### Harness CD Community Edition:
- Docker Desktop minimum version 4.3.1 (72247)
-- 3GB RAM and 2 CPUs is the minimum.
-- Docker Compose (included in Docker Desktop).
- 20GB of free disk space.

### Quickstart:
- GitHub account. You will use your GitHub account to pull a publicly available manifest (https://github.com/kubernetes/website/blob/main/content/en/examples/application/nginx-app.yaml).
 
- Docker Compose Kubernetes is installed and running in Docker Desktop (a new installation of Docker Desktop might need to have Kubernetes enabled in its **Settings**).
 
- Docker Compose Kubernetes should have at least 2GB memory and 1 CPU. That will bring the total Docker Desktop resources up to a minimum of **5GB and 3 CPUs**.

**NOTE**: If you want to use Minikube instead of Docker Desktop Kubernetes, use Minikube minimum version v1.22.0 or later installed locally. Minikube needs 4GB and 4 CPUs:```minikube start --memory 4g --cpus 4```

- Kubernetes cluster. This is the target cluster for the deployment you will set up in this quickstart. When Docker Compose Kubernetes is installed it comes with a cluster and the **default** namespace. You don't need to make any changes to Docker Compose Kubernetes.
 
**NOTE**: Don't have a cluster? See [Notes](https://docs.harness.io/article/ltvkgcwpum-harness-community-edition-quickstart#notes).

**NOTE**: Instead of relying on a Kubernetes Cluster provided by some outside provider, we'll be setting up our own Kubernetes Cluster using K3D (Kubernetes inside Docker). See also "K3d - How to run Kubernetes cluster locally using Rancher K3s" at https://www.youtube.com/watch?v=mCesuGk-Fks and our own repository for K3D at https://github.com/vanHeemstraSystems/k3d-headstart

- Review Harness CD Community Edition Overview and Harness Key Concepts to establish a general understanding of Harness.
 
**NOTE**: The Docker Compose installer is described below, but Harness also supports a [Helm installer](https://github.com/harness/harness-cd-community/blob/main/helm/README.md).

### Completely New to Continuous Delivery (CD)?

Simply put, CD is the automation of a software release process. In Harness, you model this process as a Pipeline.

What do I need for a CD Pipeline?

- An artifact to deploy: an artifact is the application or microservice you are deploying. It can be a Docker image, a zip file, etc.
- A deployment method: this is whatever specification or manifest is needed by the deployment platform you are using, such as a Kubernetes manifest.
- A place to deploy it: this is your target environment, such as a Kubernetes cluster.
 
Harness takes care of the rest.

## 300 - Architecture Summary

See [README.md](./300/README.md)

## 400 - Step 1: installation

## 500 - Step 2: Create Pipeline

See [README.md](./500/README.md)

## 600 - Step 3: Deploy

See [README.md](./600/README.md)

## 700 - Clean Up

See [README.md](./700/README.md)

## 800 - Community and Support

See [README.md](./800/README.md)

## 900 - Upgrades

See [README.md](./900/README.md)

## 1000 - Next Steps

See [README.md](./1000/README.md)

## 1100 - Notes

See [README.md](./1100/README.md)
