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

## Docker Basic Commands

``docker image ls``
This command lists all the Docker images available on your machine, providing details such as the repository, tag, image ID, and size of each image.

``docker image pull centos:latest``
This command pulls the latest version of the CentOS image from the Docker Hub repository, downloading and storing it locally on your machine.

``docker container ls``
This command lists all the running Docker containers on your machine, displaying information such as the container ID, image used, command executed, container status, and assigned names.

``docker container stop <containername>``
This command stops a running Docker container specified by its name or container ID. It sends a termination signal to the container, allowing it to gracefully stop and release its resources.

``docker container exec -it <containername> bash``
This command allows you to execute an interactive shell session (bash) inside a running Docker container. The -it flags allocate a pseudo-TTY and keep STDIN open, enabling an interactive session with the container.

``docker container stop <containername>``
This command stops a running Docker container specified by its name or container ID. It sends a termination signal to the container, allowing it to gracefully stop and release its resources.

``docker container start <containername>``
This command starts a previously stopped Docker container specified by its name or container ID. The container resumes from the state it was in before it was stopped.

Remove a container:
``docker container rm <containername>``
This command removes a Docker container specified by its name or container ID. The container must be stopped before it can be removed. This command permanently deletes the container and frees up the resources associated with it.

```bash
docker container run -it -p 3000:3000 node bash
```
> This Command Run Container with Interactive mode and expose port 3000
> and run bash command inside this node container

- after entering interactive mode you can run any command inside the container

```bash
apt update 
apt upgrade
apt install nano

```

- Setup Our App 

```bash
mkdir app && cd app && touch index.js && nano index.js
npm i express
```

```js
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hello, World!');
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});


```

- Now you can run it ``node index.js``

- ``docker commit conatinerName mytestimage`` : this command will create image from container