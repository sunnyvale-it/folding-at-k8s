To build this image:

```console
$ docker build -t sunnyvale/folding-at-k8s:1.0 .
```

To test this image:

```console
$ docker run \
    --rm \
    -ti \
    -v $(pwd)/data:/var/lib/fahclient \
    -v $(pwd):/etc/fahclient \
    sunnyvale/folding-at-k8s:1.0
```


To push this image:

```console
$ docker push sunnyvale/folding-at-k8s:1.0 
```