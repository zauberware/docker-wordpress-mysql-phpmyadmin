# Wordpress & MySQL & PHPMyAdmin running on docker

This is a tiny ready to go boilerplate for a wordpress website running with Docker. 

It uses the following libraries:

* MySQL https://github.com/docker-library/mysql
* Wordpress https://github.com/docker-library/wordpress
* PHPMyAdmin https://github.com/phpmyadmin/docker

Access your page under http://0.0.0.0:8000 after installation.

## INSTALL

### Fast way

Install and start Docker https://docs.docker.com/engine/installation/

```
$ git clone git@github.com:zauberware/docker-wordpress-mysql-phpmyadmin.git

$ mv docker-wordpress-mysql-phpmyadmin wordpress-on-docker && cd wordpress-on-docker

$ source install.sh
```
or run 

```
$ docker-compose up
```

### 1. Install Docker

Please install Docker: https://docs.docker.com/engine/installation/

Make sure that your current development workplace folder is available for mounting. Check this in your Docker Settings.

### 2. Clone repository

Clone the repository from Bitbucket and go into the project folder.

```
$ git clone git@github.com:zauberware/docker-wordpress-mysql-phpmyadmin.git

$ mv docker-wordpress-mysql-phpmyadmin wordpress-on-docker && cd wordpress-on-docker

```

Like you see there is only the wp-content folder of wordpress and few Docker files. So we use Docker to run our website for development and we are linking the wp-content folder to the wp-content folder on the Docker instance.

### 3. Install Docker & project setup

1. Start docker in the docker desktop App
2. run `source install.sh` or `docker-compose up`
3. wait for installation and check your running containers with `docker ps`. You should see wordpress, mysql and phpadmin as a container.

Page available: http://0.0.0.0:8000/
PHPMyAdmin available: http://0.0.0.0:8080/

Shut down your containers with
```
$ docker-compose down
```

## Different Setup ??

This is just a starter template. If you want to learn more about Docker templates you should visit https://docs.docker.com/develop/ . We can also recommend this repository: https://github.com/webdevops/php-docker-boilerplate

## Authors

* Simon Franzen (zauberware technologies)
* Lisa Schmitz (zauberware technologies)


![zauberware technologies](https://avatars3.githubusercontent.com/u/1753330?s=200&v=4)
