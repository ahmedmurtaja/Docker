# Docker Day 0 : OS Introduction and Prerequisite

## OS Introduction

- An operating system (OS) is system software that manages computer hardware, software resources, and provides common services for computer programs.

> So Simply , an OS is just a piece of code

- The OS is an essential component of the system software in a computer system. Application programs usually require an operating system to function.

-  other Definition :An operating system or OS is system software that works as an interface between hardware components and end-user. It enables other programs to run. Each computer system, whether it is desktop, laptop, tablet, or smartphone, all must have an OS to provide basic functionalities for the device. 

## So What is the components of the Computer or lets say the server ?

- The computer is made up of 3 main components :

1. CPU : Central Processing Unit
2. Memory : RAM
3. Storage : Hard Disk

- The CPU is the brain of the computer, it is responsible for executing the code and doing the calculations.

- The Memory is the place where the CPU stores the data that it is working on, it is much faster than the storage but it is much more expensive and it is volatile which means that if the power goes off the data will be lost.

- The Storage is the place where the data is stored, it is much slower than the memory but it is much cheaper and it is non-volatile which means that if the power goes off the data will not be lost.

- The CPU and the Memory are connected together with a very fast connection, but the storage is connected with a much slower connection.

> So how CPU and Memory and Storage are connected together ?

- The CPU and the Memory and the Storage are connected together with a bus, the bus is a set of wires that connect the CPU and the Memory and the Storage together.



<details>
<summary>The bus is made up of 3 parts</summary>

1. Address Bus : The address bus is a set of wires that the CPU uses to tell the Memory and the Storage where to read or write the data.

2. Data Bus : The data bus is a set of wires that the CPU uses to send or receive the data from the Memory and the Storage.

3. Control Bus : The control bus is a set of wires that the CPU uses to tell the Memory and the Storage what to do.

Example : If the CPU wants to read the data from the Memory, it will put the address of the data on the address bus, then it will tell the Memory to read the data by putting a signal on the control bus, then the Memory will read the data and put it on the data bus, then the CPU will read the data from the data bus.

</details>

<hr>



- in Single-core CPUs: The CPU can only execute one instruction at a time, so if we want to run multiple programs at the same time we need to switch between them very fast, so the CPU will execute a small part of the first program then switch to the second program and execute a small part of it then switch to the third program and so on, and it will keep switching between the programs very fast so it will look like all the programs are running at the same time.

- The switching between the programs is done by the OS, so the OS is responsible for managing the CPU and the Memory and the Storage.

## So what is Cache ?

- The Cache is a very fast memory that is located inside the CPU, it is used to store the data that the CPU is working on, so the CPU can access it very fast.

- The Cache is much faster than the Memory, but it is much smaller than the Memory.

- The Cache is divided into 3 levels :

1. L1 : The fastest and the smallest level.

2. L2 : Slower and bigger than L1.

3. L3 : Slower and bigger than L2.

So whats the three levels of cache ?

- The CPU will first check if the data is in the L1 cache, if it is there then it will use it, if it is not there then it will check the L2 cache, if it is there then it will use it, if it is not there then it will check the L3 cache, if it is there then it will use it, if it is not there then it will check the Memory, if it is there then it will use it, if it is not there then it will check the Storage, if it is there then it will use it, if it is not there then it will load it from the Storage to the Memory then use it.

- So the CPU will first check the L1 cache, then the L2 cache, then the L3 cache, then the Memory, then the Storage.
 

>After All of this , What is the OS ?

>The OS is a piece of code that manages the CPU and the Memory and the Storage, it is responsible for running the programs and managing the resources.

## So what is the Kernel ?

- The Kernel is the core of the OS, it is the part of the OS that manages the CPU and the Memory and the Storage.

- The Kernel runs in the supervisor mode, so it has full access to the CPU.

- The Kernel is the part of the OS that runs in the ring 0, so it has full access to the hardware.

### What is the ring 0 ?

- The ring 0 is the most privileged level, it has full access to the hardware and the memory and the CPU.

![](https://fawzi.wordpress.com/files/2009/05/four-protection-rings.png)

### How the kernel is related to the OS ?

- The Kernel is the core of the OS, it is the part of the OS that manages the CPU and the Memory and the Storage.

## So what is the Shell ?

- The Shell is a program that runs in the user mode, it is the part of the OS that interacts with the user.

### What is the user mode ?

- The user mode is the least privileged level, it has limited access to the hardware and the memory and the CPU. 
- ring 3 is the user mode.
- ring 0 is the kernel mode.

### back to the shell ?

- we can say that the shell is the interface between the user and the kernel.

- we can execute commands using the shell, and the shell will execute the commands using the kernel.

## What is the process ?

- A process is a program that is running on the computer.

- A process is made up of 3 parts :

1. Code : The code is the instructions that the CPU will execute.

2. Data : The data is the data that the CPU will work on.

3. Stack : The stack is used to store the local variables and the return addresses.

- The process is stored in the Memory.

- The process is executed by the CPU.

- The process is managed by the OS.

processes are managed by the OS, so the OS is responsible for creating the processes and destroying the processes and switching between the processes.

<!-- ## What is the thread ? -->

  
<!-- CPU -->
<!-- Memory -->
<!-- Storage -->
<!-- Cache -->
<!-- L1 -->
<!-- L2 -->
<!-- L3 -->
<!-- Address Bus -->


