# Cloud Infrastructure Report

## 1. Operating System

The cloud server is running **Ubuntu Linux**.

## 2. Kernel Version

The Linux kernel version is **6.8.0-136-generic**.

## 3. CPU Model

The CPU model is **Intel Xeon E312xx (Sandy Bridge) @ 2.0GHz**.

## 4. CPU Architecture

The CPU architecture is **x86_64**, which is a 64-bit system architecture.

## 5. Number of CPU Cores

The server has **1 CPU core**.

## 6. Total RAM

The server has **1.9 GiB of total RAM**.

## 7. Disk Capacity

The primary disk has a total capacity of **19.4 GiB**. The main filesystem `/dev/vda1` has **5.4 GiB used** and **13 GiB available**, with 30% of the storage currently used.

## 8. Mounted File Systems

The server has several mounted file systems:

| Filesystem   |  Size | Used | Available | Use % | Mount Point |
| ------------ | ----: | ---: | --------: | ----: | ----------- |
| `/dev/vda1`  | 19.4G | 5.4G |       13G |   30% | `/`         |
| `/dev/vda16` |  881M | 117M |      639M |   15% | `/boot`     |
| `/dev/vda15` |  105M | 6.2M |       99M |    6% | `/boot/efi` |
| `tmpfs`      |  191M | 996K |      190M |    1% | `/run`      |
| `tmpfs`      |  952M |  84K |      952M |    1% | `/dev/shm`  |
| `tmpfs`      |  5.0M |    0 |      5.0M |    0% | `/run/lock` |

## 9. Hostname

The hostname of the cloud server is **ubuntu**.

## 10. IP Address

The primary IP address of the server is **172.30.1.2/24**.

The server also has a Docker bridge IP address of **172.17.0.1/16**.

## Conclusion

The investigation showed that the KillerCoda environment is a Linux-based cloud server running Ubuntu. It has an x86_64 architecture, an Intel Xeon processor with one CPU core, 1.9 GiB of RAM, and a 19.4 GiB primary disk. The server also uses mounted filesystems for the operating system, boot files, and temporary runtime data. Its primary network address is 172.30.1.2/24, while the Docker bridge provides an additional internal network address.
