# midterm-Lab-Exam-


# Mission 6: Cloud Deployment Engineer

# Mission Overview

This laboratory activity demonstrates on how to deploy a two-tier private cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as the database.

## Objectives

- Understand two-tier application architecture.
- Create a Docker Compose YAML configuration file.
- Deploy Nextcloud and MariaDB containers.
- Verify running containers and access the Nextcloud setup page.
- Document deployment commands and Infrastructure as Code principles.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs app
docker-compose logs database
docker-compose down
```

## Skills Learned

- Creating and editing YAML files using nano.
- Verifying application status and reading container logs.
- Documenting cloud deployments using Markdown.


- `compose-deployment.png` — containers running.
- `nextcloud-web.png` — Nextcloud setup page.
- `compose-teardown.png` — containers stopped and removed.

#Conclusion

This mission introduced Infrastructure as  a Code and showed how Docker Compose simplifies the deployment and management of multi-container applications.
