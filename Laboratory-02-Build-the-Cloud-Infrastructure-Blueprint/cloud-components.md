# Cloud Infrastructure Components

## 1. Compute Resources

### Purpose

Compute resources provide the processing power needed to run applications, programs, and services.

### Importance in Cloud Computing

Compute resources are important because applications need CPU and memory to process tasks. Cloud providers allow organizations to increase or decrease computing resources depending on their needs.

### KillerCoda Example

The KillerCoda Linux server provides compute resources through its CPU and RAM. The server has an Intel Xeon E312xx processor, 1 CPU core, and approximately 1.9 GiB of RAM.

CPU: Intel Xeon E312xx
CPU cores: 1
RAM: 1.9 GiB

## 2. Storage Resources

### Purpose

Storage resources are used to save operating system files, applications, user data, and other information.

### Importance in Cloud Computing

Storage is important because cloud applications need a place to store data. Cloud storage also allows organizations to keep and access information without depending only on local physical storage.

### KillerCoda Example

The KillerCoda server has a main filesystem `/dev/vda1` with a capacity of 19G. It has approximately 5.4G used and 13G available. Other mounted filesystems include `/boot` and `/boot/efi`.

/dev/vda1
19G total
5.4G used
13G available

## 3. Networking Resources

### Purpose

Networking resources allow computers, servers, and other devices to communicate with each other.

### Importance in Cloud Computing

Networking is important because cloud servers need network connections to communicate with users, applications, databases, and other cloud services.

### KillerCoda Example

The KillerCoda server uses the network interface `enp1s0`. Its IP address is `172.30.4.94`, which allows the Linux environment to participate in network communication.

Network interface: enp1s0
IP address: 172.30.4.94

## 4. Operating System

### Purpose

An operating system manages the computer's hardware and provides an environment where applications and other software can run.

### Importance in Cloud Computing

The operating system is important because cloud applications and services need an operating environment. Linux is commonly used for cloud servers because it is flexible, reliable, and widely supported.

### KillerCoda Example

The KillerCoda environment is running Ubuntu 24.04.4 LTS. The Linux operating system manages the server's CPU, memory, storage, networking, and other resources.

## Summary

| Component | KillerCoda Example | Main Purpose |
|---|---|---|
| Compute | Intel Xeon CPU, 1 CPU core, 1.9 GiB RAM | Processes tasks and runs applications |
| Storage | `/dev/vda1`, 19G | Stores files and data |
| Networking | `enp1s0`, IP `172.30.4.94` | Allows network communication |
| Operating System | Ubuntu 24.04.4 LTS | Manages hardware and software |
