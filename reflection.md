# Mission Reflection

Completing Mission 6 helped me understand how Docker Compose can simplify the deployment of cloud applications. Before this Lab activity, I  understood  that Docker could run individual containers, but I did not fully understand how multiple containers could work together as one application. Through this mission.
Writing a `docker-compose.yml` file makes a cloud engineer's job easier because all the required services and configurations are defined in one place. Instead of manually creating and connecting containers using several commands, an engineer can use one Compose command to start the entire application. This approach saves time, reduces repetitive work, and makes deployments easier to reproduce.

I also learned that YAML indentation is very important. If I accidentally use a tab instead of spaces or place a line at the wrong indentation level, Docker Compose may report a configuration error. This taught me to check the structure of my file carefully before deploying the application.

Environment variables, such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_HOST`, help configure the application and database. They tell Nextcloud which database to use and provide the connection details it needs. However, I also learned that real passwords should be protected and should not be published in a public repository.

Deploying Nextcloud made me feel more confident because I could see how different services work together in a real-world application. It showed me that cloud storage systems require more than just a website; they also need a database and proper communication between components.

This mission helped me appreciate automation, containerization, and organized documentation. In the future, I want to improve my skills in Docker, cloud security, networking, and persistent storage so I can deploy more reliable applications.

Overall, this activity taught me that planning, testing, and documenting infrastructure are important responsibilities of a cloud engineer.
