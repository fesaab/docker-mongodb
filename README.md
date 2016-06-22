# docker-mongodb
Automatically put up and running the latest MongoDB server with Docker

## Description
Simple Dockerfile for install and run the latest instance of MongoDB Community Edition.

## Usage
Copy the Dockerfile to a directory and build it running:

```
docker build -t saab/mongodb:1.0.0
```

After the build finish you can run it with:

```
docker run --name mongodb -i -t -p 27017:27017 saab/mongodb:1.0.0
```

OBS: the above command will start attached to the mongod process. To detach from the container just hit CTRL+P followed by CTRL+Q.