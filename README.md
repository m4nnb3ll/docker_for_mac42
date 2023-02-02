# How to use a docker in a simple practical way in your MacOS
A light guide on how to use docker in your 42 MacOS(For me it's CatalinaOS)

### Install docker from MSC(Managed Software Center)

<p align="center"> <img src="https://github.com/m4nnb3ll/docker_for_mac42/blob/images/1.png" alt="docker installation on MSC" /> </p>

### Install [42-wizzard](https://github.com/0xShady/42_wizzard)

<p align="center"> <img src="https://github.com/m4nnb3ll/docker_for_mac42/blob/images/f2.jpg" alt="42 wizzard installation" /> </p>

### Run the following in the terminal
```
42 -docker
```
The command will change Docker to your goinfre

### Now that docker is installed, run it

<p align="center"> <img src="https://github.com/m4nnb3ll/docker_for_mac42/blob/images/2.png" alt="running docker" /> </p>

### Open terminal and follow along
#### Run a container based on an image that you want, for me i chose `debian`
**Go to the directory that you want to share with your docker container** and do the following:
```
docker run -tdv $(pwd):/root/ --name deb_container debian
```
#### Get inside the container that you just run
Go to an empty terminal, for example you can split terminal in your VSCode:

<p align="center"> <img src="https://github.com/m4nnb3ll/docker_for_mac42/blob/images/3.jpg" alt="vscode terminal" /> </p>

and do the following:
```
docker exec -it deb_container bash
```
#### Once you are inside the container, you can then install the programs that you want
Let's install `valgrind` for example:
<p align="center"> <img src="https://github.com/m4nnb3ll/docker_for_mac42/blob/images/4.jpg" alt="vscode terminal" /> </p>
