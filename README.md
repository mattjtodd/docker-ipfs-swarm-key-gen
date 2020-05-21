# Dockerized ipfs-swarm-key-gen app

This is a really simple dockerized version of the Swarm key generator provided by [Kubuxu/go-ipfs-swarm-key-gen](https://github.com/Kubuxu/go-ipfs-swarm-key-gen).


It builds down to a binary of ~2.5M


Published to DockerHub @ [docker.io/mattjtodd/ipfs-swarm-key-gen](https://hub.docker.com/repository/docker/mattjtodd/ipfs-swarm-key-gen)


## Alternative Method

As this is really a simple file which just uses a random hex encoded string, the following could also be used:

`docker run --rm -it alpine:3.11 echo "/key/swarm/psk/1.0.0/"; echo "/base16/"; openssl rand -hex 32;`

