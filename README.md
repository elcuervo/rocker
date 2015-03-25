
_the docker, docker-machine and docker-compose wrapper_

![](http://wac.450f.edgecastcdn.net/80450F/wkdq.com/files/2013/03/Rock-Hand-Sign-Credit-iStockphoto-141325118.jpg?w=600&h=0&zc=1&s=0&a=t&q=89)

Rocker is an opinionated wrapper around some of the docker toolkit.

It wraps some of the behaviour to allow a more seamless transition between
docker hosts.

## Install

```bash
./configure
make install
```

## Usage

```bash
# Bootstrap your environment:
rocker bootstrap

# Check the status of your env:
rocker check

# Run docker-compose commands with the current env:
rocker compose

# Run docker-machine commands with the current env:
rocker machine

# Get the current env
rocker current

# Get the current env IP address
rocker ip

# List your docker hosts
rocker ls

# Any command that is not from rocker and it's from docker can be run directly
# and it will use the alredy defined environment.
rocker ps
rocker info

# If there are any overlapping you can always run:
rocker do [docker command]
```
