# Origin
Originally based on https://github.com/wmnnd/nginx-certbot

# Complete Docker cerbot generator for Let’s Encrypt certificates

> This repository is accompanied by a [step-by-step guide on how to
set up nginx and Let’s Encrypt with Docker](https://medium.com/@pentacent/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71).

`init-letsencrypt.sh` fetches and ensures the renewal of a Let’s
Encrypt certificate for one or multiple domains in a docker-compose
setup with nginx.
This is useful when you need to set up nginx as a reverse proxy for an
application.

## Installation
1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose).

2. Open ports 443 and 80 in your firewall

3. Clone this repository: `git clone https://github.com/sys7emx/docker-certbot.git`

4. Run the init script:

        ./init-letsencrypt.sh example.com www.example.com

5. Run the server:

        docker compose up

6. The certificates will be in the certbot folder

## License
All code in this repository is licensed under the terms of the `MIT License`. For further information please refer to the `LICENSE` file.
