# [BXA](https://johannesbuchner.github.io/BXA/) container:

If you find PyMultiNest enables your research, please consider citing my publication to give back for the time invested:
[Buchner et al. 2014, A&A](http://www.aanda.org/articles/aa/abs/2014/04/aa22971-13/aa22971-13.html)

## Default beaviour of the container:
Launched without option this container run the command: none

# Where to start

## Install docker:
Short version (may not be the last version):
  Fedora/RedHat:

        $ sudo dnf install docker

## Run docker daemon:
  Fedora/RedHat:

        $ sudo systemctl start docker

Complete story:
[Install docker](https://docs.docker.com/engine/installation/)

## Run an interactive shell in a container:

  Short version:
        docker run -t -i \<container_ID\> /bin/bash

        docker run -t -i ubuntu /bin/bash

Links to the [official docker documentation](https://docs.docker.com/):

[Docker basics](https://docs.docker.com/engine/userguide/basics/)


# Build your hown BXA container:


## Clone the BXA git repo:

        $ cd <work_space>
        $ git clone https://github.com/ldouchy/docker_BXA.git

## Build a container:

  Short version:
        docker build \<path_to_the_Dokerfile\>

## Run the build:

        $ docker build -t <TAG> .

  You should obtain the container ID:

        Successfully built e553342157db

[Build a container](https://docs.docker.com/reference/builder/)


## Run the container with an interractive shell

        $ sudo docker run -t -i e553342157db /bin/bash


# How to customized your installation:

## Customize the Dockerfile to add your own code

## Save your BXA instance:


# HEASoft links

[official documentation page](https://johannesbuchner.github.io/BXA/)

[General install guide](https://heasarc.gsfc.nasa.gov/docs/software/lheasoft/install.html)

