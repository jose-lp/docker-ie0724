# Imagen base ubuntu 18.04
FROM ubuntu:20.04

# Mantainer
LABEL maintainer="José López Picado"
LABEL email="joselp1695@gmail.com"

# Instalación de paquetes
RUN apt update && apt install -y  --no-install-recommends  \
        build-essential \
        git \
        libbz2-dev \
        libreadline-dev \
        libsqlite3-dev \
        libssl-dev \
        zlib1g-dev \
        libffi-dev \
        python3-dev \
        python3-pip \
        make \
    && rm -rf /var/lib/apt/lists/*

# Instalación de bibliotecas de python
RUN pip3 install pyinstaller