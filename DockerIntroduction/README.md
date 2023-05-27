# Docker Introduction

<p align="center">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

## What is Docker?

Docker is a computer program that performs operating-system-level virtualization, also known as “containerization”.

<p align="center">
  <img src="https://github.com/ahmedmurtaja/Docker/assets/56529633/974b0860-2074-4250-8e07-9176c3c9d02f" alt="Docker" />
</p>


> Simply its a toy box with all the toys you need to play with.

### So what is containerization or container?

Containerization is a lightweight alternative to full machine virtualization that involves encapsulating an application in a container with its own operating environment.

<!-- gif![7nb6y0](https://github.com/ahmedmurtaja/Docker/assets/56529633/7076d595-cb2e-4a2e-b34f-4fffe81db49e)
 2 still not understand -->

<p align="center">
  <img src="https://github.com/ahmedmurtaja/Docker/assets/56529633/7076d595-cb2e-4a2e-b34f-4fffe81db49e" alt="Docker" />
</p>

So Suppose, for instance, that two apps both use Node but have various versions. In a solitary setting, they may run beside one another without interfering with one another.

so we can say that container is a isolated environment for running an application.

<!-- bold -->
###  <b>So Docker is a VM ?  </b>


<p align="center">
  <img src="https://github.com/ahmedmurtaja/Docker/assets/56529633/f6944e37-bd3b-42db-b2ff-2e76d13013f1" alt="Docker" />
</p>


No, Docker is not a VM. Docker is a containerization platform which packages your application and all its dependencies together in the form of containers so as to ensure that your application works seamlessly in any environment be it development or test or production.

## What the difference between VM and Docker?

### First, let's understand two terms:
- kernel
- Hypervisor

### Kernel

A kernel is the central part of an operating system. It manages the operations of the computer and the hardware, most notably memory and CPU time. 

<b> its main job is to manage the communication between the software and the hardware. </b>

<hr>

### Hypervisor or Virtual Machine Monitor (VMM) 

A hypervisor is a program that allows multiple operating systems to share a single hardware host. Each operating system appears to have the host's processor, memory, and other resources all to itself.

<hr>

### So what is the difference between VM and Docker?

- Docker is a containerization platform which packages your application and all its dependencies together in the form of containers so as to ensure that your application works seamlessly in any environment be it development or test or production.

![container](https://github.com/ahmedmurtaja/Docker/assets/56529633/c67ec6e8-684b-41e9-8326-569432a3cbed)

<hr>

- A virtual machine (VM) is an operating system (OS) or an application that enables you to run multiple operating systems on the same physical hardware machine, and in a secure, isolated environment.

![VM](https://github.com/ahmedmurtaja/Docker/assets/56529633/66d6ce18-e1a0-4f63-9959-65ea16c9744c)


A container runs natively on an OS and shares the kernel of the host machine with other containers. It runs a discrete **process**, taking no more memory than any other executable, making it lightweight.

By contrast, a virtual machine (VM) runs a full-blown “guest” operating system with virtual access to host resources through a hypervisor. In general, VMs incur a lot of overhead beyond what is being consumed by your application logic.

<hr>

|            | Containers                                             | Virtual Machines (VMs)                                       |
|------------|--------------------------------------------------------|-------------------------------------------------------------|
| Technology | Docker, Kubernetes, containerization platforms         | VMware, Hyper-V, Xen, virtualization platforms                |
| Isolation  | Lightweight isolation                                  | Strong isolation                                             |
| Resource   | Shares host OS kernel, minimal duplication              | Emulates complete OS, duplication of OS and system resources |
| Overhead   | Lower resource overhead, faster startup times           | Higher resource overhead, slower startup times               |
| Portability | Highly portable, easy to deploy across different hosts | Less portable, tied to specific virtualization platform      |
| Scalability | Easy to scale horizontally and vertically              | Scaling depends on virtualization platform capabilities      |
| Use Cases  | Microservices, distributed applications                | Legacy applications, different OS requirements               |
| Performance| Better performance due to reduced overhead              | Slightly reduced performance due to virtualization layers    |

Source: [Docker vs. VMs](https://www.docker.com/resources/what-container)

<hr>

### So why container is faster in booting up than VM?
> Because docker container is just a process that runs on the host machine, so it doesn't need to boot up a whole OS.

> While VM is a whole OS that runs on the host machine, so it needs to boot up the whole OS.

### why creating a container is faster than creating a VM?

> because we dont need hypervisor to create a container, while we need hypervisor to create a VM.

<hr>

![image](https://github.com/ahmedmurtaja/Docker/assets/56529633/d7037c05-4da2-4f34-9bb7-fd5e2a930695)




