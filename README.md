# docker-browser-sync

A simple way of running [browser-sync](https://www.browsersync.io/) without having to install [node](https://nodejs.org/)

## Build the docker image

```
$ docker build -t <your-image-name> .
```

## Run the image with local directory as the webroot

```
$ docker run -p 3000:3000 -it --mount type=bind,source="$(pwd)"/src,target=/usr/src/app/src <your-image-name>
```
