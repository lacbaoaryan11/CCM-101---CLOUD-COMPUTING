# Laboratory 03 – Multi-Cloud Explorer

This laboratory explores and compares Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP).


# Laboratory 03 – Multi-Cloud Explorer

## Checkpoint 7 – Linux Investigation

For this checkpoint, I used an Ubuntu Linux environment in the KillerCoda Playground. I used Linux commands to identify the operating system, CPU information, memory, and disk space.

---

## 1. Operating System

I used the following command to identify the operating system:

```bash
cat /etc/os-release
```


The command showed that the server is running **Ubuntu Linux**.

The version shown by my terminal is:

Ubuntu 24.04.4 LTS (Noble Numbat)



![Operating System]

---

## 2. CPU Information

I used the following command to check the CPU information:

```bash
lscpu
```

The command displayed information about the processor, including its architecture, number of CPUs, and CPU model.

Important information from my terminal:

Architecture: x86_64
CPU(s): 1
CPU Model: Intel Xeon E312xx (Sandy Bridge, IBRS update)
CPU Speed: 2.00 GHz
Thread(s) per core: 1
Core(s) per socket: 1
Socket(s): 1

### Screenshot

![CPU Information]

---

## 3. Memory

I used the following command to check the system memory:

```bash
free -h
```

The command displayed the total, used, and available memory of the Ubuntu server.

Important information from my terminal:

Total Memory: 1.9 GiB
Used Memory: 413 MiB
Free Memory: 869 MiB
Available Memory: 1.5 GiB
Swap: 1.0 GiB

### Screenshot

![Memory Information]

---

## 4. Disk Space

I used the following command to check the available disk space:

```bash
df -h
```

The command displayed the total disk space, used space, available space, and percentage of disk space being used.

Important information from my terminal:

Filesystem: /dev/vda1
Total Disk Space: 19G
Used Space: 5.4G
Available Space: 13G
Usage: 30%
Mounted on: /


![Disk Space]

---

## 5. Cloud Migration

If this Linux server were migrated to the cloud, it could be hosted using virtual machine services from AWS, Microsoft Azure, and Google Cloud Platform.

### AWS

The Linux server could be hosted using **Amazon EC2**. Amazon EC2 provides virtual servers that can run Linux operating systems and different types of workloads.

### Microsoft Azure

The Linux server could be hosted using **Azure Virtual Machines**. Azure Virtual Machines allow users to create and run Linux-based virtual machines in the cloud.

### Google Cloud Platform

The Linux server could be hosted using **Compute Engine**. Compute Engine provides virtual machines that can run Linux operating systems and applications.

### Cloud Service Comparison

| Cloud Provider        | Service That Could Host the Linux Server |
| --------------------- | ---------------------------------------- |
| AWS                   | Amazon EC2                               |
| Microsoft Azure       | Azure Virtual Machines                   |
| Google Cloud Platform | Compute Engine                           |

## Conclusion

The Linux server can be migrated to any of the three major cloud platforms because AWS, Azure, and GCP all provide virtual machine services that support Linux. The best choice would depend on the organization's requirements, budget, existing technologies, and preferred cloud platform.
