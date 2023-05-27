# Docker Introduction

<p align="center">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

## What is Docker?

Docker is a computer program that performs operating-system-level virtualization, also known as “containerization”.

<!-- insert gif 1  -->

> Simply its a toy box with all the toys you need to play with.

### So what is containerization or container?

Containerization is a lightweight alternative to full machine virtualization that involves encapsulating an application in a container with its own operating environment.

<!-- gif 2 still not understand -->

So Suppose, for instance, that two apps both use Node but have various versions. In a solitary setting, they may run beside one another without interfering with one another.

so we can say that container is a isolated environment for running an application.

<!-- bold -->
###  <b>So Docker is a VM ?  </b>

<!-- shoot him img -->

No, Docker is not a VM. Docker is a containerization platform which packages your application and all its dependencies together in the form of containers so as to ensure that your application works seamlessly in any environment be it development or test or production.

## What the difference between VM and Docker?

### First, let's understand two terms:
- kernel
- Hypervisor

### Kernel

A kernel is the central part of an operating system. It manages the operations of the computer and the hardware, most notably memory and CPU time. 

<b> its main job is to manage the communication between the software and the hardware. </b>

### Hypervisor or Virtual Machine Monitor (VMM) 

A hypervisor is a program that allows multiple operating systems to share a single hardware host. Each operating system appears to have the host's processor, memory, and other resources all to itself.

### So what is the difference between VM and Docker?

- Docker is a containerization platform which packages your application and all its dependencies together in the form of containers so as to ensure that your application works seamlessly in any environment be it development or test or production.


- A virtual machine (VM) is an operating system (OS) or an application that enables you to run multiple operating systems on the same physical hardware machine, and in a secure, isolated environment.


