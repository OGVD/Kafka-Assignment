# Kafka-Assignment
To create the environment for the assignment:

1. Build the docker image by executing the appropriate command in the base repository folder:

    - **Linux/Windows**:
      ```bash
      docker build -t kafka-jupyter .
      ```
    - **macOS**:
      ```bash
      docker build -t kafka-jupyter . --file=Dockerfile_mac
      ```

2. Run the container.

    ```bash
    docker run -p 8888:8888 -p 9092:9092 -p  2181:2181 kafka-jupyter
    ```

3. Enter the jupyter notebook link that appears when running the container.


To stop the environment:

1. List all running containers.

    ```bash
    docker ps
    ```

2. Copy the Container ID and stop it.

    ```bash
    docker stop CONTAINER_ID
    ```