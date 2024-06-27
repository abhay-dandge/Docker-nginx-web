---

This repository contains the setup for hosting a web application using NGINX within a Docker container. The project is designed to provide a consistent and isolated environment for serving web files, making deployment and scaling straightforward and efficient.

### Features
- **Dockerized NGINX**: The project uses Docker to encapsulate the NGINX web server, ensuring a consistent setup across different environments.
- **Simple Deployment**: The Docker setup simplifies the process of deploying your web application, allowing you to get started quickly.

### Getting Started
1. **Clone the Repository**: Download the project files from the repository.
   ```bash
   git clone https://github.com/abhay-dandge/Docker-nginx-web
   cd your-nginx-docker-repo
   ```
2. **Build the Docker Image**: Use the provided Dockerfile to build the Docker image.
   ```bash
   docker build -t my-nginx-app .
3. **Create a vloume to store the code
   ```bash
    mkdir /nginx/data -p
   
   ```
5. **Run the Docker Container**: Start a container from the built image, mapping the necessary ports.
   ```bash
   docker run --name my-nginx-container -v /nginx/data:/usr/share/nginx/html -p 8080:80 -d my-nginx-app
   ```
6. **Access Your Web Application**: Open a web browser and navigate to `http://localhost:8080` to see your web application in action.


By following these instructions, you can quickly set up and run your web application using NGINX in a Docker container, ensuring a reliable and consistent environment for development and deployment.

---
