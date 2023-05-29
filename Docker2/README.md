# Docker Architecture and Basic Commands

## Docker Engine Architecture

![image](https://github.com/GSG-G13/Docker/assets/56529633/345bd90d-f466-4716-b15f-764083031d5e)

- Docker is made up of 3 main components :

1. Docker Client : The Docker Client is a command line tool that is used to interact with the Docker daemon.

2. Docker Daemon : The Docker Daemon is a background process that runs on the host machine. its like a server that is responsible for creating the images and running the containers.

3. Docker Registry : The Docker Registry is a place where we can store our images.

- Docker is a client-server application.

So the Docker Client will send commands to the Docker Daemon, and the Docker Daemon will execute the commands and send the output to the Docker Client.

## Docker Engine

![image](https://github.com/GSG-G13/Docker/assets/56529633/e2ccc990-4d67-489a-92c0-4fdda8b6d80e)

> Remember that process is a program that is running on the computer.

### what is shim ?

- shim is a process that is used to manage the container.

For example, when we run the command `docker run hello-world`, the Docker Client will send the command to the Docker Daemon, and the Docker Daemon will create a shim process, and the shim process will create the container.

-shim keep listening to the container, and when the container stops, the shim will stop.




