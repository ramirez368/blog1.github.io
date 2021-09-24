---
layout: default
---





[//]: #  There should be whitespace between paragraphs

[//]: #  There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# What is Docker?

  Docker is an open platform for developing, shipping, and running applications, it enables you to separate your applications from your company infrastructure so you can deliver software faster. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running pushing it to production.


![Docker Diagram](https://res.cloudinary.com/practicaldev/image/fetch/s--pfrqBBqs--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/6xpc9lwxcpkf3as9e1vi.jpeg)
[Video with More Docker.....](https://www.youtube.com/watch?v=rOTqprHv1YE)


## About the Docker Platform:
   Docker provides the ability to package and run an application in a  semi-loose and isolated environment, which is called a container. The isolation and security allow you to run many containers simultaneously on a given host. Containers are lightweight and contain everythin needed to run the application, so you do not need to rely on what is currently installed on the host. You can easily share containers while you work, and be sure that everyone you share with gets the same container that works in the same way, we have been expose tho this on the pertheneus server lab.

* Docker provides tooling and a platform to manage the lifecycle of your containers
* Develop your application and its supporting components using containers
* The container becomes the unit for distributing and testing your application.

## What can I use Docker for?
Consider the following example scenarios:

* Your developers write code locally and share their work with their colleagues using Docker containers.
* They use Docker to push their applications into a test environment and execute automated and manual tests.
* When developers find bugs, they can fix them in the development environment and redeploy them to the test environment for testing and validation.
* When testing is complete, getting the fix to the customer is as simple as pushing the updated image to the production environment.

### Installation of Docker in Windows 10 (That is what I have....)
## Before some Requirements:
Docker for Windows runs on 64-bit Windows 10 Pro, Enterprise, and Education; 1511 November update, Build 10586 or later. Docker plans to support more versions of Windows 10 in the future.

## Installation Steps
* Download Docker from https://docs.docker.com/desktop/windows/install/
* Double-click InstallDocker.msi to run the installer.
* Follow the Install Wizard: accept the license, authorize the installer, and proceed with the install.
* Click Finish to launch Docker.
* Docker starts automatically.
* Docker loads a “Welcome” window giving you tips and access to the Docker documentation.
That’s it!

## Verification
The whale in the status bar indicates a running (and accessible via terminal) Docker instance.
Open PowerShell or your favorite Windows terminal (e.g., Command prompt) and enter docker run hello-world.
From PowerShell (or your favorite Windows terminal), check the versions of docker, docker-compose, and verify your installation:
```
PS C:\Users\username> docker --version
PS C:\Users\username> docker-compose --version
PS C:\Users\username> docker-machine --version
```

## Top 16 docker commands

1.	**docker ps**  list running containers. 
2.	**docker ps -a** list all container including stopped container
3.	docker pull  download a image from Docker Hub registry. Link to the docker image is always shown on the right at dockerhub.
4.	docker build  is used to build your own container based on a Dockerfile. Common use is docker build . to build a container based on the Dockerfile in the current directory (the dot). docker build -t "myimage:latest" . creates a container and stores the image under the given name
5.	docker images or docker image ls shows all local storage images
6.	docker run  Run a docker container based on an image, i. e. docker run myimage -it bash. If no local image can be found docker run automatically tries to download the image from Docker hub.
7.	docker logs display the logs of a container, you specified. To continue showing log updates just use docker logs -f mycontainer
8.	docker volume ls  lists the volumes, which are commonly used for persisting data of Docker containers.
9.	docker network ls - list all networks available for docker container
10.	docker network connect adds the container to the given container network. That enables container communication by simple container name instead of IP.
11.	docker rm   removes one or more containers. docker rm mycontainer, but make sure the container is not running
12.	docker rmi  removes one or more images. docker rmi myimage, but make sure no running container is based on that image
13.	docker stop   stops one or more containers. docker stop mycontainer stops one container, while docker stop $(docker ps -a -q) stops all running containers. 
14.	docker start - starts a stopped container using the last state
15.	docker update --restart=no updates container policies, that is especially helpful when your container is stuck in a crash loop
16.	docker cp to copy files from a running container to the host or the way around. docker cp :/etc/file . to copy /etc/file to your current directory.




```
### Useful commands
Then we will open Firefox ok and we're going to go to localhost and there we go we have an Apache - default page now we can also access this anywhere on our network okay.

### Step 3

```



### I hope this was useful to how to setup and running of Docker


```
Thank you readers, and wait for Blog 1 next week.
For Contact e-mail me at ramirez368@hotmail.com

```
