[![Project-Docker_Workflow](https://circleci.com/gh/dSalazar10/Project-Docker_Workflow.svg?style=shield)](https://app.circleci.com/pipelines/github/dSalazar10/Project-Docker_Workflow)

# Project-Docker_Workflow
Udacity's Cloud DevOps Nanodegree Course 4 Project

Part 1 - Containerizing an application with Docker

1) Setup a local development environment
- Installed python
- Build and executed packages

2) Developed a Makefile to automate the build process
- Setup local environment using bash scripts

![](screenshot-01.png)

- Installing packages using pip3
- Testing python code using pytest
- Validating build configurations using CircleCI

![](screenshot-02.png)

- Linting Dockerfile with hadolint
- Linting python file with pylint
3) Containerize a python app using Docker
- Local build and verify packages installed successfully
`docker build --tag=app .`

![](screenshot-03.png)

- Check to see that it was built successfully
`docker image ls`
- Run the docker to see if it was setup properly
`docker run -p 80:80 app`
- Deploy Docker image to AWS Elastic Container Registry

![](screenshot-04.png)

To run the Docker image in your server, just execute the following code:
- `docker pull 966289448295.dkr.ecr.us-west-2.amazonaws.com/docker_workflow:latest`
- `docker run 966289448295.dkr.ecr.us-west-2.amazonaws.com/docker_workflow`

[Part 2](https://github.com/dSalazar10/Project-Kubernetes_Workflow)
