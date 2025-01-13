## 🌐 [English Version of README](README_EN.md)

# Docker for Developers (with Docker Swarm and Kubernetes)

This project is a comprehensive Docker course, covering everything from basic concepts to advanced usage, including Docker Swarm and Kubernetes. The content includes container creation, images, and the use of Docker Compose, as well as container orchestration with Docker Swarm and Kubernetes.

## 🔨 Project Features

### Visual Example of the Project

This project allows you to create and orchestrate containers with Docker, using different orchestration methods such as Docker Swarm and Kubernetes. It also includes creating networks and volumes, along with an example of integration using Docker Compose.

## ✔️ Techniques and Technologies Used

- **Docker**: Containers, Images, Volumes, Networks, Bind Mounts.
- **Docker Compose**: Orchestration of multiple containers.
- **Docker Swarm**: Orchestration of containers in a cluster.
- **Kubernetes**: Orchestration of containers with Kubernetes clusters.
- **YAML**: Configuration definition for containers and services.
- **Flask**: Web framework for application container examples.

## 📁 Project Structure

- **1_imagens_e_containers/**
  - **Dockerfile**: File to build the Docker image.
  - **app.js**: Simple Node.js application.
  - **copia/**: Directory with a copy of the app.js file.
  - **package.json**: Node.js dependencies.
  
- **2_volumes/**
  - **Dockerfile**: File to build an image with volumes.
  - **index.php**: Simple PHP application example.
  - **messages/**: Directory with message files.
  - **process.php**: PHP file for processing data.

- **3_networks/**
  - **1_externa/**: Contains an example of an external network in Docker.
  - **2_host/**: Example of a host network.
  - **3_conn_containers/**: Example of containers connected in a network.

- **4_yaml/**
  - **app.py**: Example of using YAML with Flask.
  - **test.yaml**: YAML configuration file.

- **5_compose/**
  - **docker-compose.yaml**: Configuration for orchestration with Docker Compose.

- **6_kubernetes/**
  - **Dockerfile**: Docker file for building a Kubernetes image.
  - **app.py**: Flask application for running on Kubernetes.
  - **templates/**: Directory with HTML template files for Kubernetes.

- **7_docker_yt/**
  - **Dockerfile**: Docker file for YouTube application.
  - **index.js**: Node.js application code.
  - **package.json**: Dependencies for the Node.js project.

- **LICENSE**: Project license.
- **README.md**: Main project documentation.
- **README_EN.md**: English documentation.
- **Slides do curso de Docker.pdf**: Course presentations.

## 🛠️ Running the Project

To run the project locally, follow the steps below:

1. **Make sure Node.js is installed**:
   - [Node.js](https://nodejs.org/) is required to run the project. You can check if it is installed by running:

   ```bash
   node -v
   ```

- If not installed, download and install the recommended version.

2. **Clone the Repository**:
    - Copy the repository URL and run the following command in the terminal:

   ```bash
   git clone <REPOSITORY_URL>
   ```

## 🌐 Deploy

To deploy the project, you can use Docker, Docker Compose, or Kubernetes, as described in the configuration files.

### Deploy with Docker

1. Navigate to the project directory.
2. Build the Docker image:

   ```bash
   docker build -t image-name .
   ```

3. Run the container:

   ```bash
   docker run -p 3000:3000 image-name
   ```

### Deploy with Docker Compose

1. Navigate to the `5_compose/` directory.
2. Create and start the containers with Docker Compose:

   ```bash
   docker-compose up --build
   ```

### Deploy with Kubernetes

1. Navigate to the `6_kubernetes/` directory.
2. Start the Kubernetes service:

   ```bash
   kubectl apply -f flask-service.yaml
   ```

3. Access the service in your browser to view the running project.
