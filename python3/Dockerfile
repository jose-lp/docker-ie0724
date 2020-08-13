# Imagen base ubuntu 18.04
FROM ubuntu:20.04

# Mantainer
LABEL maintainer="José López Picado"
LABEL email="joselp1695@gmail.com"

# Instalación de paquetes
RUN apt update && apt install -y  --no-install-recommends  \
        python3 \
        python3-pip \
        make \
    && rm -rf /var/lib/apt/lists/*

# Instalación de bibliotecas de python
RUN pip3 install pyinstaller