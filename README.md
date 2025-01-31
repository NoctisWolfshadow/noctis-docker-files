# My Docker Compose Files

## Install Docker and Docker Compose

```bash
curl -fsSL https://get.docker.com -o get-docker.sh 
sh get-docker.sh
```

## Get your Docker Compose File

Download or copy the File from this repository. Then edit it to fit your needs.
I will also provide how i use them normally further down below.
If you need multiple of these modules you should merge these files together.
Also if you merge them define CONTAINER_NAME in the file. It makes things easier.

## Run Docker Compose

If your file is not named docker-compose.yaml you need the flag -f with a Filename.
If you want to run it in detached mode add the -d Flag.
It could look like this:

```bash
docker compose -f <FILENAME> up -d
```

### Postgres

If you started the Postgres container in detached mode you can access it with
the following command:

```bash
docker exec -it <CONTAINER_NAME|CONTAINER_ID> psql -U postgres -d <DATABASE>
```

You just need to replace the CONTAINER_NAME with the name of the container or
the CONTAINER_ID with the ID of the container.
You can look up the CONTAINER_ID with the command `docker ps`.
