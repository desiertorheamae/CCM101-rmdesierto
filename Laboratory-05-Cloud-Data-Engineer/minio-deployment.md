# MinIO Deployment

## Docker Command Used

The MinIO Object Storage server was deployed using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
Web Console Port

The MinIO Web Console was accessed through port 9001. This port was entered in the KillerCoda Custom Ports or Traffic / Ports section to open the MinIO Console in a web browser.

Port 9000 was used for the MinIO server, while port 9001 was used to access the web console.

Bucket Created

A bucket named client-photos was created using the MinIO Web Console. A sample file was uploaded to the bucket to verify that the storage server was working properly.

Environment Variables

The -e flags in the Docker command were used to set environment variables for the MinIO server.

The MINIO_ROOT_USER variable set the administrator username to cloudadmin, while the MINIO_ROOT_PASSWORD variable set the administrator password to CloudNova2026!. These credentials were used to log in to the MinIO Web Console.
