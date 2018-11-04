[![Build Status](https://travis-ci.org/gurkalov/ubuntu-ssh.svg?branch=master)](https://travis-ci.org/gurkalov/ubuntu-ssh)
[![BCH compliance](https://bettercodehub.com/edge/badge/gurkalov/ubuntu-ssh?branch=master)](https://bettercodehub.com/)

Get Started
-----

The images are built by [Docker hub](https://hub.docker.com/r/gurkalov/ubuntu-ssh/).

To run an SSH daemon in a Ubuntu 18.04 LTS (Bionic Beaver)
container:

    docker run -d -p 2222:22 -e SSH_KEY="$(cat ~/.ssh/id_rsa.pub)" gurkalov/ubuntu-ssh:bionic

To connect to this container as root:

    ssh -p 2222 root@localhost
    
 