# About Folding@K8S

Folding@K8S is the Sunnyvale's effort to port the [Folding@Home](https://foldingathome.org) client on Kubernetes.

The idea is fairy simple: donate the unused Kubernetes cluster CPUs to help finding cures for diseases like cancer, ALS, Parkinson’s, Huntington’s, Influenza and lately COVID-19.

We packaged the FAHClient in a Docker image, available on DockerHUB following this repo [sunnyvale/folding-at-k8s](https://hub.docker.com/repository/docker/sunnyvale/folding-at-k8s)

# How to get started

## Deploy on top of a Kubernetes cluster

We leveraged [Helm](https://helm.sh) packaging system to streamline the deployment procedure on your Kubernetes cluster. To install **Folding@K8S** on a Kubernetes cluster please refer to this  [README.md](helm/README.md).

In this case, using a **DeamonSet** K8S resource we deploy a single-container Pod on each cluster node. 

## Simply using Docker

You can help folding using Docker or a Docker Swarm cluster.
To run the client as a Docker container, please refer to this  [README.md](docker/README.md)
