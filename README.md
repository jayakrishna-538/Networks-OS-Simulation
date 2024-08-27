# Networks-OS-Simulation

This repository encompasses a collection of six distinct projects, each of which encompasses several additional smaller projects within itself.



# FTP Implementation using TCP Sockets #

This project implements a File Transfer Protocol (FTP) using TCP sockets in C++. 

The server waits for a connection from the client, and once connected, the client can perform various file operations such as PUT, GET, MPUT, and MGET.

These operations allow the transfer of .txt and .c files between the client and server, with support for overwriting files based on user input.

The IP address and port number are provided via command-line arguments.

# Wireshark Analysis of Video Uploading to YouTube #

We identified and described key protocols and their packet formats.

Explained the sequence of messages and any handshaking involved.

Calculated metrics like throughput, RTT, and packet loss at different times of the day.

# Inter Process Communication #

This project contains three mini projects related to Inter Process Communication

### Directory Merging ###

There are two directories available, and the goal is to move the combined set of files from both directories into each of the directories.

This has been achieved using pipes.

### Online Exam System ###

The aim is to administer an online examination for students using communication through child processes. In this setup, students utilize child processes, while the parent process serves as the coordinator.

The child processes are responsible for responding to questions, and the parent process manages the collection and evaluation of these answers. Subsequently, individual grades are presented to each student.

### Event Registration ###

The objective is to build the multi-threaded event registration system for a convention centre which organizes e events concurrently and has a capacity of c.

Queries involved in this are:

~~~
1. Inquire the number of seats available in 'a' events

2. Book k tickets in 'a' events

3. Cancel a booked ticket
~~~


# Multi threading #

This project contains three mini projects which aims to solve some real world problems with the help of threads and some lock variables or semaphores.

### Restaurant Problem ###

A restaurant has a capacity of N. The constraints are as follows:

~~~
• A diner cannot enter until the restaurant has opened its front door to let people in.

• The restaurant cannot start service until N diners have come in.

• The diners cannot exit until the back door is open.

• The restaurant cannot close the backdoor and prepare for the next batch until all the diners of the previous batch have left.
~~~

### Bridge Problem ###

A bridge connects north and south bound people of a village. If both side people enter the bridge on the same time, then deadlock occurs. 

To prevent the deadlock, concurrency is implemented using threads and mutex locks or semaphores.

Two cases are considered in this:

~~~
➢ Case 1 : Consider the scenario in which northbound people prevent southbound
           people from using the bridge, or vice versa.

➢ Case 2 : Consider the scenario in which northbound people don't prevent
           southbound people from using the bridge, or vice versa.
~~~

### E-Commerce App ###

The e-commerce platform handles millions of transactions per day. Many servers are running parallely on the system. 
Each server is responsible for a specific type of operations. Each server contains several worker threads.

Each worker thread has a priority level assigned to it, and a certain amount of resourcesassigned to it. 
The priority level determines the order in which the threads are scheduled to process requests.
The resources assigned to each thread determine the maximum number of requests it can handle simultaneously.

The objective is to develop a scheduling algorithm that handles the transaction load.
