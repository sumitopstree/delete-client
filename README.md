PS C:\Users\anand> docker.exeker^C
PS C:\Users\anand> docker version
Client:
 Version:      17.03.1-ce-rc1
 API version:  1.27
 Go version:   go1.7.5
 Git commit:   3476dbf
 Built:        Wed Mar 15 20:33:22 2017
 OS/Arch:      windows/amd64

Server:
 Version:      17.03.1-ce-rc1
 API version:  1.27 (minimum version 1.12)
 Go version:   go1.7.5
 Git commit:   3476dbf
 Built:        Wed Mar 15 20:28:18 2017
 OS/Arch:      linux/amd64
 Experimental: true
PS C:\Users\anand> docker-compose version
docker-compose version 1.11.2, build f963d76f
docker-py version: 2.1.0
CPython version: 2.7.13
OpenSSL version: OpenSSL 1.0.2j  26 Sep 2016
PS C:\Users\anand> docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
sumitanand17/test   v1                  387f0125b623        5 days ago          428 MB
mongo               4.0.4               525bd2016729        13 days ago         383 MB
keymetrics/pm2      8                   24e97c9d11cd        11 months ago       90.1 MB
PS C:\Users\anand> docker run -idt --name mongo -p 27017:27017 mongo:4.0.4
c3abbccafea0753983e6ad4adcf4054e9dc691bd6f9d4a601acf862ac1bf2f1b
PS C:\Users\anand> docker ps
CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS
            NAMES
c3abbccafea0        mongo:4.0.4         "docker-entrypoint..."   5 seconds ago       Up 4 seconds        0.0.0.0:27017->
