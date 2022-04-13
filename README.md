# Getting Started

A simple application to run on docker

### running the application without docker compose

We will be using `docker run` to be able to run **getting-started**, follow the line below to be able to run the service:

```bash
docker run -dp 80:80 docker/getting-started
```

After running the command access `localhost:80` so you can view the application running.

### running the application with docker composer

We will use docker-compose to be able to run the script already prepared to be able to run the service in docker, follow the example below of what is expected to be in the file:

```yaml
version: "3.9"
services:
  get-started:
    image: docker/getting-started
    ports:
      - 80:80
```

Only this is enough for us to run the service, if everything is ok, run the command below:

```bash
docker-compose up -d
```

After running the command access `localhost:80` so you can view the application running.

Everything being in agreement you have already managed to run your first service in docker.
