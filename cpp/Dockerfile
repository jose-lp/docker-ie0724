# Imagen base ubuntu 18.04
FROM ubuntu:20.04

# Mantainer
LABEL maintainer="José López Picado"
LABEL email="joselp1695@gmail.com"

ENV DEBIAN_FRONTEND=noninteractive

# Instalación de paquetes
RUN apt update && apt install -y  --no-install-recommends  \
        build-essential \
        make \
        cmake \
        libgtest-dev \
    && rm -rf /var/lib/apt/lists/*

# Configuracipon de gtest
RUN cd /usr/src/gtest \
    && cmake CMakeLists.txt \
    && make \
    && cp *.a /usr/lib
