---
layout: default
---



[More About Docker](https://www.youtube.com/watch?v=rOTqprHv1YE).

[//]: #  There should be whitespace between paragraphs

[//]: #  There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# What is Docker?

  Docker is an open platform for developing, shipping, and running applications, it enables you to separate your applications from your company infrastructure so you can deliver software faster. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running pushing it to production.

## The Docker Workflow:

![Lamp Stack Diagram](https://res.cloudinary.com/practicaldev/image/fetch/s--pfrqBBqs--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/6xpc9lwxcpkf3as9e1vi.jpeg)


## About the Docker Platform:

   Docker provides the ability to package and run an application in a  semi-loose and isolated environment, which is called a container. The isolation and security allow you to run many containers simultaneously on a given host. Containers are lightweight and contain everythin needed to run the application, so you do not need to rely on what is currently installed on the host. You can easily share containers while you work, and be sure that everyone you share with gets the same container that works in the same way, we have been expose tho this on the pertheneus server lab.

* Docker provides tooling and a platform to manage the lifecycle of your containers:

Develop your application and its supporting components using containers.
The container becomes the unit for distributing and testing your application.
When you’re ready, deploy your application into your production environment, as a container or an orchestrated service. This works the same whether your production environment is a local data center, a cloud provider, or a hybrid of the two


## Installation Steps for LAMP Stack
### Step 1

First thing we're going to do here is we're going to update our pachages in Ubuntu, that is what we are working on and we're going to say sudo apt-get update keep putting your password and we're just going to update everything, once is done we're going to install Apache okay so we'll say sudo apt-get install apache2 ok we're going to say yes.


```js
**Linux commands For Step 1**
sudo apt-get update 
sudo apt-get install apache2 

```
### Step 2
Then we will open Firefox ok and we're going to go to localhost and there we go we have an Apache - default page now we can also access this anywhere on our network okay.

### Step 3
Next we will go ahead and install PHP so we'll say sudo apt-get install php 5, say yes, after that we will restart apache with sudo /etc/init.d/apache2 restart, now I want to test it, so we'll test PHP out okay so let's do sudo nano /var/www.html/”nameofyourfile.php”
There we’ll type <?php php echo ‘It Works’; ?> then save it on your vim editor and if you type localhost/test.php in our example in your url it should display it….It Works!


```ruby
**Linux commands For Steps 3**
sudo apt-get install php 5
sudo /etc/init.d/apache2 restart
sudo nano /var/www.html/"nameofyourfile".php
<?php php echo ‘It Works’; ?>
localhost/test.php 

```
### Step 4
So now we want to move on to MySQL so we're going to say sudo apt-get install mysql-server, at one point it would ask to set a root password to go to it it we do: 
mysql -u root -p it would ask you for the root password and once entered it would take you to mysql>, from there we could create a database by doing create database testdb;
To see it we can do show databases -> ;

```ruby
**Linux commands For Steps 4**
sudo apt-get install mysql-server
mysql -u root -p 
create database testdb
show databases -> ;
```
### Step 5
Last step would be to install the  I want to do is install PHP myadmin, so we do: 
sudo apt-get install php myadmin, it would ask you what type of server we have, you   select apache2, it would show you the configuration and ask you to set a password for php myadmin and then your root mysql password, after all these we test it but we found a few issues.

```ruby
**Linux commands For Steps 5**
sudo apt-get install php myadmin
```
## Issues when Installing/Running Apache and php:
   We found some issues when we tried to go in the url to localhost/phpMyAdmin to solve this issue we will have to edit a file so we go by typing /etc/php5/apache2.php.ini and we  need to remove the semicolon at the extension=msql.so this should be under ==Module setting== in the page. After this we will restart apache by doing:
Sudo /etc/init.d/apache2 restart, then we reload the web browser and still having issues, so the final resolution was to edit the config file for apache by going again to:
/etc/apache2/apache2.config and at the bottom and on the editor we add:
Include /etc/phpMyAdmin/apache.conf and then we restart Apache and it works.
Username should be root and the password the password that you created.




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
