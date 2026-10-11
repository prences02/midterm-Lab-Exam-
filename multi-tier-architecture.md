# Multi-Tier Architecture

# What Is a Two-Tier Architecture?

The two-tier architecture is a system divided into two main parts: the web/application tier and the database tier. These tiers communicate with each other to provide a services to users.

# The Web/Application Tier

The web/application tier handles user requests and displays the website through an web browser. In this mission, Nextcloud is the application that allows users to upload, download, organize, and manage their files.

# The Database Tier

The database tier stores important informations, such as user accounts, file metadata, and application settings. In this mission, MariaDB acts as the database for Nextcloud.
  
  # Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. Each container has its own responsibility and can be updated or restarted separately. This architecture also makes it easier to scale an application when more users need the service.

# Architecture Summary

- Web/Application Tier: Nextcloud
- Database Tier: MariaDB
- Communication: Docker Compose creates a network that allows the Nextcloud container to reach MariaDB using the service name `database`.
