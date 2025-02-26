# Ansible-Docker Microservices Infrastructure Management

## Project Overview
This project demonstrates how to set up and manage microservices using *Docker, Docker Compose, and Ansible. It includes deploying an **NGINX service* as a containerized microservice, automated configuration using Ansible, and infrastructure management.

## Features
- Containerized NGINX service using Docker.
- Infrastructure automation using Ansible.
- Configurable deployment with Docker Compose.
- Easily scalable and maintainable setup.

## Technologies Used
- *Docker* - For containerization of microservices.
- *Docker Compose* - To manage multiple containerized services.
- *Ansible* - For configuration management and deployment automation.
- *NGINX* - As a web server to test the microservices setup.

## Project Structure

|-- ansible-setup/
    |-- inventory                  # Ansible inventory file
    |-- deploy-nginx.yml           # Ansible playbook for deploying NGINX
    |-- docker-compose.yml         # Docker Compose configuration
    |-- ansible_docker_project.zip # Zipped project file


## Setup Instructions
### Prerequisites
Ensure you have the following installed:
- Docker
- Docker Compose
- Ansible
- Git (for uploading to GitHub)

### 1. Clone the Repository
bash
git clone https://github.com/your-username/your-repository.git
cd your-repository


### 2. Running the Docker Compose Setup
bash
docker-compose up -d

This will start the NGINX container.

### 3. Verify the Deployment
Open your browser and visit:

http://localhost:8080

If you see the NGINX welcome page, your setup is working!

### 4. Deploy Using Ansible
bash
ansible-playbook -i inventory deploy-nginx.yml

This will configure and deploy the NGINX service using Ansible.

## Troubleshooting
- If you get a permission error while running Docker commands, use sudo.
- If NGINX does not start, check the Docker container logs:
bash
sudo docker logs <container_id>


## Uploading to GitHub
To upload the project ZIP file to GitHub, follow these steps:
bash
git add ansible_docker_project.zip
git commit -m "Added project ZIP file"
git push origin main


## Conclusion
This project sets up a basic *CI/CD pipeline* for microservices using *Docker and Ansible*. It helps automate deployment and infrastructure management, making it easier to scale applications.
