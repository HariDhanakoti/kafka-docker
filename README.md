#Create docker images with docker compose yaml

- Pull zookeeper image from docker hub
- Pull kafka image from docker hub
- 'Zookeeper' container
  - To expose port 2181
- 'Kafka' container
  - To wait until the zookeeper is up and started
  - To expose port 29092 internally and 9092 externally
- Init kafka container
  - To wait until the kafka container is up and started
  - With help of the 'entrypoint' run the 'command' to create kafka topics
