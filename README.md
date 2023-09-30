# docker-postgres

A simple Postgres container for `docker` (or `podman`).

To use with Docker, you should be able to run the standard `docker-compose` commands `docker-compose up` and `docker-compose down`. You should also be able to comment out the `podman` section in the `start` and `stop` scripts and uncomment the `docker` parts if you want.

## Instructions

1. To start the container, run the `start` script.
2. To stop the container, run the `stop` script.
3. To create a systemd service file, run the `./systemd-container-service-file-generate` script
   - Use the `--podman` flag to generate a systemd service file that will run `podman` while using `docker-compose` as the container orchestrator.
