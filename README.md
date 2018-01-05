# CentOS Pupy

Single layer Dockerfile for n1nj4sec's Pupy RAT running under CentOS

## Usage:  
```
docker run -i -t -p $HOSTIP:$HOSTPORT:$CONTAINERPORT {docker image ID}

# Or, to use a local path to pass data out of your container:
docker run -i -t -v /path/to/host/folder:/tmp/loot -p $HOSTIP:$HOSTPORT:$CONTAINERPORT {docker image ID}

# To detach from your container once it's running:
ctl + p + ctl + q

# To reattach:
docker attach {container ID or name}

# To expose multiple ports on your container, add multiple instances of the "-p" argument:
... -p $HOSTIP:$HOSTPORT:$CONTAINERPORT -p $HOSTIP:$HOSTPORT:$CONTAINERPORT ...

```
