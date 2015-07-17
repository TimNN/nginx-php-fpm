## Introduction
This is a Dockerfile to build a container images based on nginx and php-fpm. It is a simplified version of [ngineered/nginx-php-fpm](https://github.com/ngineered/nginx-php-fpm).

### Git reposiory
The source files for this project can be found here: [https://github.com/TimNN/nginx-php-fpm](https://github.com/TimNN/nginx-php-fpm)

If you have any improvements please submit a pull request.
### Docker hub repository
The Docker hub build can be found here: [https://registry.hub.docker.com/u/TimNN/nginx-php-fpm/](https://registry.hub.docker.com/u/TimNN/nginx-php-fpm/)

## Nginx Versions
- Mainline Version: **1.9.3**
- Stable Version: **1.8.0**
- *Latest = Mainline Version*

## Installation
Pull the image from the docker index rather than downloading the git repo. This prevents you having to build the image on every docker host.

```
docker pull TimNN/nginx-php-fpm:latest
```
To pull the Stable Version:

```
docker pull TimNN/nginx-php-fpm:stable
```
To pull the Mainline Version:

```
docker pull TimNN/nginx-php-fpm:mainline
```
## Running
To simply run the container:

```
sudo docker run --name nginx -p 8080:80 -d richarvey/nginx-php-fpm
```
You can then browse to http://\<docker_host\>:8080 to view the default install files.
