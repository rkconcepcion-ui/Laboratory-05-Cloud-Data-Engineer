# Storage Types Research 

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                            | Primary Use Case                                                                                      | Cloud Provider Example |
| ------------------ | ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ---------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually.    | Best used for virtual machines, operating systems, and applications that need fast disk-like storage. | AWS EBS                |
| **File Storage**   | Stores data as files organized in folders and directories.             | Best used when multiple users or applications need shared access to files.                            | AWS EFS                |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. | Best used for large amounts of unstructured data such as images, videos, backups, and documents.      | AWS S3                 |

## Why Object Storage Is Best for the Client

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It can provide scalable and accessible storage for millions of photos without storing them directly inside the web server container.

