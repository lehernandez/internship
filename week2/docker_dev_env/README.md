# Task for Week 2

The intend of this task is to run a PHP Script on PHP CLI using a Docker Container.

### Pre-requirements:
  - Ubuntu System
  - Git
  - Docker Installation
  
### Building Ubuntu Container

Clone the repository from GitHub that contains the Dockerfile

```sh
$ git clone https://github.com/lehernandez/internship.git
$ cd internship/week2/docker_dev_env
$ docker build -t ubuntu/php .
```

These commands will create a Ubuntu docker container with PHP cli installed. 
Because of the -t parameter you can identify the docker image as: ubuntu/php

Also the hello.php script will be copied to the root folder of the container


### Running the PHP CLI Script

```sh
$ docker run -t -i ubuntu/php php hello.php
```

