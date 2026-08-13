# Laboratory 02 — Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focused on investigating the basic components of cloud infrastructure. Using the KillerCoda Ubuntu environment, I examined the server's operating system, CPU, memory, storage, networking, hostname, and IP address. I also researched AWS, Microsoft Azure, and Google Cloud and created a simple cloud infrastructure diagram.

## Objectives

The objectives of this laboratory were to:

- Understand the major components of cloud infrastructure.
- Investigate hardware and software resources in a Linux environment.
- Identify compute, storage, networking, and operating system resources.
- Compare services from AWS, Microsoft Azure, and Google Cloud.
- Create a simple cloud infrastructure diagram.
- Practice technical documentation using Markdown.
- Organize and improve my GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

The major cloud infrastructure components investigated in this laboratory were:

### Compute

Compute resources provide CPU and memory for running applications and processing tasks. The KillerCoda server uses an Intel Xeon CPU with 1 CPU core and approximately 1.9 GiB of RAM.

### Storage

Storage resources are used to save operating system files, applications, and other data. The KillerCoda environment has a main `/dev/vda1` filesystem with a capacity of 19G.

### Networking

Networking allows servers and other devices to communicate. The KillerCoda server uses the `enp1s0` network interface and has the IP address `172.30.4.94`.

### Operating System

The operating system manages the server's hardware and software. The KillerCoda environment uses Ubuntu 24.04.4 LTS.

## Tools Used

The following tools were used during this laboratory:

- KillerCoda Playground
- Ubuntu Linux
- Linux terminal
- GitHub
- Markdown
- Web browser
- Diagramming tool

## Linux Commands Executed

The following Linux commands were used to investigate the cloud server:

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
hostname
hostname -h
ip addr
df -h

These commands were used to identify the operating system, kernel, CPU, CPU cores, RAM, hostname, IP address, network interfaces, and storage information.

Skills Learned

During this laboratory, I learned how to investigate a Linux server using basic terminal commands. I also learned how compute, storage, networking, and operating systems work together in cloud infrastructure. Additionally, I improved my Markdown documentation, GitHub organization, cloud service comparison, and basic infrastructure diagramming skills.

Challenges Encountered

One challenge I encountered was understanding the different Linux commands and the information displayed by each command. I also had to learn how to organize the files and screenshots correctly in GitHub. Another challenge was understanding the equivalent infrastructure services provided by AWS, Microsoft Azure, and Google Cloud.

Conclusion

This laboratory helped me understand the basic infrastructure behind cloud computing. By investigating a Linux environment and documenting the results, I gained a better understanding of how compute, storage, networking, and operating systems work together to support cloud services.
