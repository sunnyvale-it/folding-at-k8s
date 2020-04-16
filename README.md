

## Prerequisites


```console
$ 
```



To test the installation (this will not alter your system at all)

```console
$ helm install sunnyvale-it-folding-at-k8s \
    --dry-run \
    --debug \
    --set image.pullPolicy=Always
    --set image.version="1.0" \
    --set fold.config.anonymousFolding="false" \
    --set fold.config.processingPower="low" \
    --set fold.config.team="Sunnyvale S.r.l." \
    --set fold.config.user="Sunnyvale_S.r.l." \
    --set fold.config.httpServerListenAddresses="0.0.0.0" \
    --set fold.config.commandServerListenAddresses="0.0.0.0" \
    --set fold.config.passkey="keep it secret" \
    ./helm/sunnyvale-it-folding-at-k8s
```

```console
$ helm install sunnyvale-it-folding-at-k8s \
    --debug \
    --set image.pullPolicy=Always
    --set image.version="1.0" \
    --set fold.config.anonymousFolding="false" \
    --set fold.config.processingPower="low" \
    --set fold.config.team="Sunnyvale S.r.l." \
    --set fold.config.user="Sunnyvale_S.r.l." \
    --set fold.config.httpServerListenAddresses="0.0.0.0" \
    --set fold.config.commandServerListenAddresses="0.0.0.0" \
    --set fold.config.passkey="keep it secret" \
    ./helm/sunnyvale-it-folding-at-k8s
```

```console
$ helm delete sunnyvale-it-folding-at-k8s
```
