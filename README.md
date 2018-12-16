# Verdaccio docker-compose

[Using Verdaccio Docker Image](https://verdaccio.org/docs/en/docker)

## Installation

Set chown to directory `verdaccio` to user verdaccio

```bash
chown -R 100:101 /path/verdaccio/conf
chown -R 100:101 /path/verdaccio/storage
chown -R 100:101 /path/verdaccio/plugins
```

Create the `.env` file from [.env.dist](.env.dist) example with the
environment variables from [docker let's encrypt nginx proxy](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion/wiki/Basic-usage)

```bash
docker-compose up -d
```

## Update docker images

```bash
./updateDockerImages.sh
```
