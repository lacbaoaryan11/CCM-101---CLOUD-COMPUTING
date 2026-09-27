# Storage Types Research

Cloud storage can be divided into three common types: Block Storage, File Storage, and Object Storage. Each type is designed for different purposes.

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in small blocks that can be accessed separately. It works like a virtual hard drive. | Operating systems, databases, and virtual machines. | AWS EBS |
| File Storage | Stores files in folders and directories. Users can access and share files through a file system. | Shared folders, documents, and files used by multiple computers. | AWS EFS |
| Object Storage | Stores data as objects together with information called metadata. Objects are stored inside buckets. | Images, videos, backups, documents, and other large amounts of unstructured data. | AWS S3 |

## Why Object Storage is Good for the Client

Object Storage is a good choice for the photo-sharing application because it can store a very large number of images without depending on the web server's local storage. It is also easy to access, organize, and scale when the number of uploaded photos increases.

## Summary

Block Storage is similar to a hard drive, File Storage works with folders and files, while Object Storage stores data as objects inside buckets. For a photo-sharing application with millions of images, Object Storage is designed to handle large amounts of unstructured data.
