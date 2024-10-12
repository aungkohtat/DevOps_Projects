# DevOps_Projects
## Project 1: Build and Deploy a Web Application Using Docker
![](/dockerized-web-app/img/docker_image_burmese_style-c40271e3-8663-4e16-b05c-d43fd223c922.jpg)
### Dockerized Web Application
- This project demonstrates how to create and deploy a containerized web application using Docker.
## Project Overview
- In this project, we'll build a simple web application using Node.js and Express, containerize it using Docker, and prepare it for deployment on a cloud platform.

## Prerequisites
- Node.js (v14 or later)
- Docker
- A Docker Hub account (for pushing the image)
- An account on a cloud platform (e.g., AWS or Azure) for deployment

## 1. Create a Simple Web App
- We've created a basic Express.js application. The main file is app.js:

## 2. Dockerfile

We use the following Dockerfile to containerize our application:

## 3. Build and Run the Container

- To build and run the container locally:

```bash
# Build the Docker image
docker build -t my-web-app .

# Run the container
docker run -p 3000:3000 my-web-app
```

## 4. Deploy on a Cloud Platform

- Instructions for deploying to AWS Elastic Container Service (ECS):

    - 1. Push your image to Docker Hub
    ```bash
        docker tag my-web-app:latest akhlab/my-web-app:latest
        docker push akhlab/my-web-app:latest
    ```
    - 2. Create an ECS cluster in the AWS Console.
    - 3. Create a task definition using your Docker Hub image.
    - 4. Create a service in your ECS cluster using the task definition.

## Key Skills 
- Docker and containerization
- Node.js and Express.js
- Cloud deployment (AWS ECS) # I already used dockerhub

## Read My Blog Posts
[Read my blog posts](https://medium.com/@alexiscloud/building-and-deploying-a-dockerized-web-application-d8e251ef8d62)

[Follow me on LinkedIn](https://www.linkedin.com/in/aungkohtat)
