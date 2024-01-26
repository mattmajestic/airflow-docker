# 🚀 airflow-docker
This repository contains a Docker container setup for [Apache Airflow](https://airflow.apache.org/), a platform to programmatically author, schedule, and monitor workflows. 

Airflow allows you to use Python to create directed acyclic graphs (DAGs) of tasks, which can be scheduled and run by the Airflow scheduler. It's a powerful tool for automating and managing complex data pipelines.

## 🏃‍♀️ To Run 
1) `docker-compose up` - This command starts up all the services defined in your docker-compose.yml file.
2) `docker ps` - This command lists all running Docker containers. You'll need the container ID for the next step.
3) `docker exec -it <container_id_from_ps> bash` - This command opens an interactive bash shell inside the running Docker container.
4) `cd ../../` - This command navigates to the root directory inside the Docker container.
5) `bash entrypoint.sh` - This command runs the entrypoint script, which should start your Airflow service.