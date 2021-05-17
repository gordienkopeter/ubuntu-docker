# Ubuntu Docker

## Getting started
```sh
# install dependencies
sudo apt install make
# install docker and docker-compose
make install user=<shared user to docker>
```

## Troubleshooting
```sh
# try to up containers
docker-compose up -d 

ERROR: Couldn`t connect to Docker daemon at http+docker://localhost - is it running? 

If it`s at a non-standard location, specify the URL with the DOCKER_HOST environment variable.

# solve
sudo systemctl restart docker

# solve with exit and reconnect
exit
ssh -i 'path/to/file.pem' user@host
```
