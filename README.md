# Frist to know

This is how you start a simple minio server and console with docker.
Using minio console with browser.
Using mc command(to review config hosts and move data).

# How to run minio

startup minio docker
```bash
docker-compose -f docker-compose.yaml down --remove-orphans --rmi local
```

shutdown minio docker
```bash
docker-compose --compatibility -f docker-compose.yaml up -d
```

# Minio information

Notice we specified the port 9000 9001 in files `docker-compose.yaml` and `ngix.conf`

We startup services: minio1, minio2, minio3, minio4, nginx

## port 9000 minio host

minio server url

http://localhost:9000

## port 9001 minio console

browser login url

http://localhost:9001/login

# Install Minio Client(mc)

https://docs.min.io/minio/baremetal/reference/minio-cli/minio-mc.html

## Linux install command
```bash
curl https://dl.min.io/client/mc/release/linux-amd64/mc --create-dirs -o $HOME/bin/mc

chmod +x $HOME/bin/mc
export PATH=$PATH:$HOME/bin/

mc --help
```

## Windows install
Download `mc.exe`
https://dl.min.io/client/mc/release/windows-amd64/mc.exe

Setup Path

# Steps(optional)

Gives you a better understanding of using minio console and mc command.

## Step 1 Create a bucketAlpha

## Step 2 Create a user

## Step 3 Login with new create user

## Step 4 Upload file to bucketAlpha

## Step 5 Create a bucketBravo

## Step 6 Review buckets

## Step 7 Move bucketAlpha data to bucketBravo

# References

https://github.com/minio/minio/tree/master/docs/orchestration/docker-compose

https://github.com/minio/minio/blob/master/docs/orchestration/docker-compose/README.md