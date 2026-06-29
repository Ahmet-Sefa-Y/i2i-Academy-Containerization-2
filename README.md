# Containerization with Docker Compose

This project was completed as part of the i2i Academy Containerization homework.

## Objective

The project demonstrates containerization by serving a custom static webpage with Nginx using Docker Compose. The same configuration was tested both locally and on a Google Cloud virtual machine.

## Technologies Used

* Docker
* Docker Compose
* Nginx
* Google Cloud Platform Compute Engine

## Project Files

* `index.html`: Custom static webpage served by Nginx.
* `docker-compose.yml`: Docker Compose configuration for the Nginx service.

## How to Run Locally

1. Clone the repository or download the project files.
2. Open a terminal in the project directory.
3. Run:

```bash
docker compose up -d
```

4. Open the following address in a web browser:

```text
http://localhost:8080
```

## Container Configuration

The Nginx container uses the `nginx:latest` image and maps port `8080` on the host machine to port `80` inside the container. The custom `index.html` file is mounted as the default Nginx webpage.

## Stop the Container

```bash
docker compose down
```
