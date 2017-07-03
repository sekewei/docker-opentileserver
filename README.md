# docker-opentileserver
=======================

### Build docker image for specific region:
docker build   -f ./Dockerfile   -t taiwan-osmbright:latest   -    <    taiwan-osmbright_v1_build.tar.gz

### Run docker container:
docker run -it -p 80:80 --name taiwan taiwan-osmbright:latest

### Look into docker container:   (use Ctrl-p q for escape)
docker exec -it  taiwan bash

### Example calls (from the host):
http://localhost/openlayers-example.html
