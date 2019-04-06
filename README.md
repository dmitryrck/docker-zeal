# Zeal

This is a docker image for [zealdocs.org](https://zealdocs.org/).

# Running

```terminal
$ docker run \
    --detach=false \
    -it \
    --rm \
    -e DISPLAY=unix$DISPLAY \
    -e GDK_DPI_SCALE \
    -e GDK_SCALE \
    -v /etc/localtime:/etc/localtime:ro \
    -v zeal_docs:/${USER} \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    dmitryrck/zeal
```

Or using x11docker:

```terminal
$ x11docker -m dmitryrck/zeal
```
