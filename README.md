# besn's Debian+Nginx+Phalcon Framework Environment (with some extras)

Simple docker image based on Debian stretch which includes nginx, PHP 7.2, Memcached and the Phalcon Framework as well as tools to bootstrap building frontend and backend applications

## Start the environment

	docker run --name <container name> besn/phalcon-environment:latest

## Run commands in the docker container

 	docker run --rm -ti besn/phalcon-environment:latest bash
    
or
    
  	docker exec -ti <container name> bash

## Use the image in your GitLab CI build

Add `image: besn/phalcon-environment:latest` to your `.gitlab-ci.yml` and use `node`, `npm`, `yarn` or `composer` commands for your build or test tasks
