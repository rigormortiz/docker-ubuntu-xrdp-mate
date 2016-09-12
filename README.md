# What is docker-ubuntu-xrdp-mate?
Docker-ubuntu-xrdp-mate is a base image of Ubuntu Xenial with the Mate desktop environment and xrdp installed. It can be used stand alone or as a base for a more personalized desktop environment. Includes Mate and Firefox

# How to use this image
You can use this image as a base for your own customized desktop environment.

For example:

```
FROM rigormortiz/ubuntu-xrdp-mate:0.1

...
```

You can also use this image as a stand alone Mate desktop environment. 

For example:

```
docker run -d -P rigormortiz/ubuntu-xrdp-mate:0.1
```

You can then use `docker ps` to figure out the port number and point your favorite RDP client at it. The default username and password is `desktop`. You can also map it to the default RDP port with `-p 3389:3389`.
