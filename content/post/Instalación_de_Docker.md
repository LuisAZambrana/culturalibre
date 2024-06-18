---
title: "Instalación de Docker"
date: 2024-06-18T13:28:39-03:00
Description: "Instalación de Docker sobre gnulinux"
Tags: [docker]
Categories: [infraestructura]
DisableComments: false
---
# Instalación de docker

A continuación paso a paso para instalar docker. Ejecutar "linea por linea"

- `sudo apt update && sudo apt upgrade`
- `sudo apt install curl python3-pip apt-transport-https ca-certificates software-properties-common`
- `sudo apt install docker.io`
- `sudo usermod -aG docker tuusuario`
- `sudo systemctl enable --now docker`
- `docker --version`
- `sudo curl -L "https://github.com/docker/compose/releases/download/2.3.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
- `sudo chmod +x /usr/local/bin/docker-compose`
- `docker-compose --version`

Si bien no hace falta es recomendable reiniciar el servidor

**Verificar:**

- `docker --version`
- `docker-compose --version`