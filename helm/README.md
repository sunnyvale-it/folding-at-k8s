# About 

Follow these steps to setup **Folding@K8S** on your Kubernetes cluster

## Prerequisites

- Install [Helm 3.x](https://helm.sh)
- Change your CWD (Current Working Directory) in the path where this README.md file resides.
- Setup a kubectl context pointing to your cluster

## Install Folding@K8S

To install **Folding@K8S** artifacts, run this command (please change all the **\<placeholder\>** elements accordingly):


- **anonymousFolding** can be true or false
- **processingPower** can be light, medium or full
- **team** contains your FAH team id (if any)
- **user** contains your FAH user name (if not folding as anonymous)
- **passkey** contains the passkey you obtained from the FAH website (if not folding as anonymous)


```console
$ helm install sunnyvale-it-folding-at-k8s \
    --debug \
    --set image.pullPolicy=Always
    --set image.version="1.0" \
    --set fold.config.anonymousFolding="<placeholder>" \
    --set fold.config.processingPower="<placeholder>" \
    --set fold.config.team="<placeholder>" \
    --set fold.config.user="<placeholder>" \
    --set fold.config.httpServerListenAddresses="0.0.0.0" \
    --set fold.config.commandServerListenAddresses="0.0.0.0" \
    --set fold.config.passkey="<placeholder>" \
    ./sunnyvale-it-folding-at-k8s
```

## Test the installation artifacts (this will not alter your Kubernetes cluster at all)

To test the installation artifacts created by Helm, just add the `--dry-run` flag in the command showed before. In this way you will not alter your Kubernetes cluster at all.

## Remove Folding@K8S from your Kubernetes cluster

```console
$ helm delete sunnyvale-it-folding-at-k8s
```
