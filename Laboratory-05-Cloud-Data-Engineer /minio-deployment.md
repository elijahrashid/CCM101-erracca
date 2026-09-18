# MinIO Deployment Documentation

**Laboratory Activity 5 — Mission 5: The Cloud Data Engineer**

## Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
pgsty/minio:latest server /data --console-address ":9001"
```

**Note on image substitution:** The lab handout specifies the `minio/minio` image, but pulling it failed with a `pull access denied` error. This is because MinIO Inc. stopped publishing new images to Docker Hub and archived the official repository. I substituted `pgsty/minio`, an actively maintained community fork that is a drop-in replacement — it accepts the same environment variables and the same `server` command, so no other part of the deployment changed.

## Web Console Access

- **Port:** 9001 (mapped via `-p 9001:9001`)
- Accessed through the KillerCoda "Traffic / Ports" panel by entering port 9001 and clicking Access.

## Bucket Created

- **Name:** `client-photos`
- Created via the MinIO web console under Buckets → Create Bucket.
- A sample file was uploaded into the bucket to confirm the deployment works end-to-end.

## Environment Variables Explained

The two `-e` flags set MinIO's admin login credentials at container startup, instead of requiring a separate configuration step afterward:

- `MINIO_ROOT_USER=cloudadmin` — sets the root/admin username used to log into the web console and authenticate API requests.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` — sets the corresponding root password. MinIO reads both variables when the container starts and uses them to initialize the admin account.

## Screenshots

- `screenshots/minio-deployed.png` — terminal output showing the container pulled and running (`docker ps`).
- `screenshots/minio-bucket-upload.png` — MinIO web console showing the `client-photos` bucket with the uploaded test file.
