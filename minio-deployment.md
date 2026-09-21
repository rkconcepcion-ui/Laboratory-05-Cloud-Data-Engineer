# MinIO Deployment

## Checkpoint 3 - Deploy an Object Storage Server

MinIO was deployed using Docker as an S3-compatible object storage server.

### Docker Command Used

The following command was used to deploy the MinIO server:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

The MinIO container was verified using:

```bash
docker ps
```

The container was running successfully with ports 9000 and 9001 mapped to the host.

## Checkpoint 4 - Access the Cloud Console and Create a Bucket

The MinIO Web Console was accessed through port:

```text
9001
```

The MinIO login credentials configured during deployment were used to access the Web Console.

A bucket named:

```text
client-photos
```

was created through the MinIO Web Console.

A sample image was uploaded successfully to the `client-photos` bucket.

### Environment Variables

The `-e` flags in the Docker command were used to set environment variables for the MinIO container.

```text
MINIO_ROOT_USER=cloudadmin
```

This sets the administrator username used to log in to the MinIO Web Console.

```text
MINIO_ROOT_PASSWORD=CloudNova2026!
```

This sets the administrator password used for authentication.

### Verification

The MinIO server was tested using:

```bash
curl -v http://localhost:9000/minio/health/live
```

The response returned `HTTP/1.1 200 OK`, confirming that the MinIO server was running successfully.

