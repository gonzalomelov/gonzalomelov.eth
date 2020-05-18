version: '3.7'

services:

  gonzalomelov: 
    image: nginx:latest
    volumes:
      - .:/usr/share/nginx/html
    network_mode: bridge
    restart: always
    ports:
      - "13000:80"
    labels:
    - traefik.frontend.rule=Host:www.gonzalomelov.com,gonzalomelov.com
    - traefik.docker.network=bridge
    - traefik.port=80