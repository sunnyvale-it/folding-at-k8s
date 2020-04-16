# About 

Follow these steps to run **Folding@K8S** as a Docker container

## Prerequisites

- Having [Docker](https://www.docker.com) installed
- Change your CWD (Current Working Directory) in the path where this README.md file resides.

# Run Folding@K8S as a Docker container

To run Folding@K8S as a Docker container:

```console
$ docker run \
    --name folding-at-k8s \
    -d \
    -ti \
    -v $(pwd)/data:/var/lib/fahclient \
    -v $(pwd):/etc/fahclient \
    sunnyvale/folding-at-k8s:1.0
```

