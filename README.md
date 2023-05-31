## This is a initial setup for Python Flask in Docker, using Nginx and Gunicorn

### There is two environments using Docker Compose:

### Development

As it uses Docker Compose, you can easily up this by running the following command in this same directory:

```sh
docker compose up -d --build
```

It will run at the localhost at 8006 port. Make sure you have the docker compose installed.

### Production

This runs two containers, the Python and the Nginx one, it uses the Gunicorn for the WSGI. You can up this by running the following command in that same directory:

```sh
docker compose -f docker-compose.prod.yml up -d --build
```

It will run at the localhost at 8006 port, be free to config nginx.conf, domain and ports as you need. It's only a quicky start kit.