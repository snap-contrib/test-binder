FROM docker.pkg.github.com/snap-contrib/docker-snap/snap:latest

USER root

ADD environment.yml /tmp/environment.yml

RUN mamba env create -n notebook -f /tmp/environment.yml

EXPOSE 8888

USER jovyan

WORKDIR /home/jovyan
