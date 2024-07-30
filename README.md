# Hyle Cairo Proving Server Tee

## Pre-requisites
### Install Docker
To install visit the Docker [website](https://www.docker.com/).

## Build the Enclave Builder image
Run these commands in the `/hyle-cairo-proving-server-tee` directory.
```bash!
docker build -t enclave .
```
## Run the docker container
```
docker run -it --privileged -v `pwd`:/app/mount enclave
```

This will generate the enclave image `.eif` file in the `/enclave` folder.
