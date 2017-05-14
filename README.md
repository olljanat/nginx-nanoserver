# nginx-nanoserver
This dockerfile uses native 64 bit version of [nginx]|(http://nginx.org) from http://nginx.kr and installs it to [microsoft/nanoserver]|(https://hub.docker.com/r/microsoft/nanoserver/) based container.
Official version of nginx cannot be used because it is 32 bit version of binary which is not supported on nano server.

## Build
```bash
docker build -t nginx-nanoserver .
```

## Run
```bash
docker run -d --name nginx -p 80:80 nginx-nanoserver
```
