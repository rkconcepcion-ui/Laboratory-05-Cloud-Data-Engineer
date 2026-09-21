# Mission Reflection

This mission helped me understand how object storage works and how Docker can be used to deploy a storage server. Object storage is better suited for storing millions of photos because it is designed to store large amounts of unstructured data such as images, videos, and documents. Unlike traditional block storage, object storage organizes data as objects with metadata and unique identifiers. It can also scale to handle a very large number of files without requiring the same type of manual storage management.

Using Docker made deploying the MinIO storage server easier because I did not have to manually install and configure all of its dependencies. With a single Docker command, I was able to download the MinIO image, create a container, configure the login credentials, and expose the required ports. Docker also made it easier to verify whether the server was running by using commands such as `docker ps` and `docker logs`.

A bucket in cloud storage is a container used to organize and store objects such as photos and other files. In this activity, I created a bucket named `client-photos` and successfully uploaded a sample image into it. This helped me understand how files are organized in object storage.

Large enterprise companies can protect their object storage data from physical server failures by using multiple copies of data, redundancy, replication, backups, and distributed storage systems. If one physical server fails, another copy can still be available, helping prevent data loss.

Finally, my confidence in navigating the Linux command line is growing. At first, some Docker commands and errors were confusing, especially when deploying MinIO. However, by checking commands, logs, container status, and health endpoints, I became more comfortable troubleshooting problems. This mission gave me practical experience with Linux, Docker, and object storage and showed me how these technologies work together in a cloud environment.

