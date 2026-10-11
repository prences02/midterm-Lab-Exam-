# Docker Compose Guide

# What Does the `services:` Block Do?

The `services:` block defines the containers that make on the application. In this mission, it defines two services: `database`, which uses the MariaDB image, and `app`, which uses the Nextcloud image.

# How Does Nextcloud Find the Database?

The environment variable `MYSQL_HOST=database` tells Nextcloud to connect to the database service named `database`.  The Docker Compose provides an network for the services, allowing the application container to resolve the database service name without needing its IP address.

Other environment variables configure the database name, username, and password so that Nextcloud can connect to MariaDB.

# Docker Run vs. Docker Compose

The `docker run` command is commonly used to create and start a individual container. When the application requires multiple containers, we may need to run several commands and manually configure on their connections.

The `docker-compose up -d` command reads the on `docker-compose.yml` file and starts all the defined services in the background. This makes  a deployment  easier to repeat, manage, and share with other engineers.

# Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

If the environment uses the newer Compose plugin, use `docker compose` instead of `docker-compose`.

## Conclusion

Docker Compose helps engineers define and deploy multi-container applications using Infrastructure as Code. It reduces repetitive manual work and makes application deployment more consistent.
