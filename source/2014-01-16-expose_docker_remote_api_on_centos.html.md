---
layout: post
title: Expose Docker Remote API on CentOS
tags: docker
lang: en
creation-date: 2014-01-16 15:59:06 +0900
modified-date: 2014-01-16 15:59:06 +0900
---
We came to install Docker on CentOS easily.
Here is an instruction for the way to expose Docker remote API port on CentOS.

    $ cat /etc/sysconfig/docker
    other_args=""

READMORE

Edit the file `/etc/sysconfig/docker` as below.

    other_args="-H tcp://0.0.0.0:4243 -H unix:///var/run/docker.sock"

After that, restart docker and try to access the host from another host.

    $ sudo /etc/init.d/docker restart
    ...
    $ curl $hostname:4243/images/json
    ...

I think docker is almost practical for production environment since it cames to run on CentOS.