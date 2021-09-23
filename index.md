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
1.Download Docker from https://docs.docker.com/desktop/windows/install/
2.Double-click InstallDocker.msi to run the installer.
3.Follow the Install Wizard: accept the license, authorize the installer, and proceed with the install.
4.Click Finish to launch Docker.
5.Docker starts automatically.
6.Docker loads a “Welcome” window giving you tips and access to the Docker documentation.
That’s it!

##Verification
The whale in the status bar indicates a running (and accessible via terminal) Docker instance.
Open PowerShell or your favorite Windows terminal (e.g., Command prompt) and enter docker run hello-world.

From PowerShell (or your favorite Windows terminal), check the versions of docker, docker-compose, and verify your installation:

```
### Useful commands
Then we will open Firefox ok and we're going to go to localhost and there we go we have an Apache - default page now we can also access this anywhere on our network okay.

### Step 3

```
### Step 4

### Step 5


## Issues when Installing/Running Apache and php:
  



| Command                          | Action                            | Fix |
|:---------------------------------|:----------------------------------|:------|
| /etc/php5/apache2.php.ini        | Type the command to edit the file | Remove extension at extension=msql.so|
| Sudo /etc/init.d/apache2 restart | It will restart Apache        | Not yet fixed
| /etc/apache2/apache2.config      |  Type this to edit the file   | Include /etc/phpMyAdmin/apache.conf |



### I hope this was useful to how to setup LAMP and being expose to more Linux


```
Thank you readers, and wait for Blog 1 next week.
For Contact e-mail me at ramirez368@hotmail.com

```
