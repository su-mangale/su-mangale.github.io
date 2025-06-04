---
title: "How to Configure GitOps with FluxCD"
date: 2025-06-04
---

FluxCD is a powerful tool for implementing GitOps in Kubernetes environments. In this post, I'll walk you through the basic steps to get started with FluxCD for continuous delivery using Git as your source of truth.

## What is GitOps?
GitOps is a modern approach to managing infrastructure and application deployments using Git repositories as the single source of truth. All changes are made via pull requests and automatically applied to your cluster by automation tools like FluxCD.

## Why Use FluxCD?
- Declarative, automated Kubernetes deployments
- Integrates with existing Git workflows
- Supports Helm, Kustomize, and plain YAML
- Secure and scalable for teams

## Getting Started
1. **Install FluxCD CLI:**
   ```sh
   curl -s https://fluxcd.io/install.sh | sudo bash
   flux --version
   ```
2. **Bootstrap Your Cluster:**
   ```sh
   flux bootstrap github \
     --owner=<your-github-username> \
     --repository=<your-repo> \
     --branch=main \
     --path=clusters/my-cluster
   ```
3. **Connect Your Git Repository:**
   - Store your Kubernetes manifests, Helm charts, or Kustomize overlays in your repo.
   - FluxCD will watch for changes and apply them automatically.
4. **Define Workloads:**
   - Add your manifests to the specified path in your repo.
   - Use `GitRepository`, `Kustomization`, or `HelmRelease` resources as needed.
5. **Monitor and Troubleshoot:**
   - Use `flux get all` to check the status of your resources.
   - View logs and events for troubleshooting.

## Resources
- [FluxCD Documentation](https://fluxcd.io/docs/)
- [GitOps Principles](https://www.gitops.tech/)


