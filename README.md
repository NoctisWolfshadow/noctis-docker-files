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

## Run Docker Compose

If your file is not named docker-compose.yaml you need the flag -f with a Filename.
If you want to run it in detached mode add the -d Flag.
It could look like this:

```bash
docker compose -f <FILENAME> up -d
```
