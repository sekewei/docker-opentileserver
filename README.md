# docker-opentileserver

## Download source files for building the docker image:
```
git clone git@github.com:sekewei/docker-opentileserver.git
cd docker-optenfileserver
```

## Build docker image for specific region:
`docker build   -f ./Dockerfile   -t taiwan-osmbright:latest   -    <    taiwan-osmbright_v1_build.tar.gz`

## Run docker container:
`docker run -it -p 80:80  --name twbright   taiwan-osmbright:latest`

## Update new map data:   (use Ctrl-p + Ctrl-q for escape)
```
docker exec -it  twbright /bin/bash
cd /opentileserver
sh ./reload-opentileserver.sh
```

## Example calls (from the host):
http://localhost/openlayers-example.html

## Consult the revision documentation
https://seke-blog.blogspot.tw/2017/04/how-to-build-osm-map-server-for-taiwan.html
