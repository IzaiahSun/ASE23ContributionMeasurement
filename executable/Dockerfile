FROM ubuntu:latest

WORKDIR /

ENV DEBIAN_FRONTEND noninteractive

RUN apt update && apt install -y git openjdk-11-jdk python3 python3-pip curl unzip graphviz

RUN mkdir joern && cd joern && \
    curl -L "https://github.com/joernio/joern/releases/latest/download/joern-install.sh" -o joern-install.sh && \
    chmod u+x joern-install.sh && \
    ./joern-install.sh

# COPY ./requirements.txt /requirements.txt

# RUN pip3 install -r /requirements.txt

COPY ./dist /script

RUN mkdir /script/projects && mkdir /script/results && mkdir /ramdisk

WORKDIR /script