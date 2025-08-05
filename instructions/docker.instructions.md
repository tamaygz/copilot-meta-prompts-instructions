# Instructions for Updating a Dockerized App

When making changes to a service in your Dockerized application, **do not use** `docker-compose restart`.  
Instead, follow these steps:

1. **Build the updated service:**
    ```
    docker-compose build {servicename}
    ```

2. **Start the service in detached mode:**
    ```
    docker-compose up -d
    ```

This ensures your changes are properly built and applied to the running containers.
Do not install or run apps locally, work with docker instead as specified.