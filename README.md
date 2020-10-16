[![noswpatv3](http://zoobab.wdfiles.com/local--files/start/noupcv3.jpg)](https://ffii.org/donate-now-to-save-europe-from-software-patents-says-ffii/)
[![noswpatv3](http://zoobab.wdfiles.com/local--files/start/noupcv3.jpg)](https://ffii.org/donate-now-to-save-europe-from-software-patents-says-ffii/)
About DockerPS (dps)
====================

It is a simple script to display IP addresses of each running container.

Copy it somewhere (for ex /usr/bin/dps), and launch some containers (here a ping to google.com)

```
zoobab@sabayon /home/zoobab/soft/docker-ps-showips [22]$ sudo docker run -d debian:wheezy ping google.com
f7d36f2b8e850c17aa3eef7b8e72e292d40dac72de335223259a5c7fb32bf226

zoobab@sabayon /home/zoobab/soft/docker-ps-showips [23]$ sudo docker run -d debian:wheezy ping google.com
a32b4e7ebf11d211252e7eab1e1105363d10bb39e6dd6dab41451ba094927a5a
```

Then run dps (you might need sudo or not):

```
zoobab@sabayon /home/zoobab [6]$ sudo dps
IP ADDRESS      CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
172.17.0.9      a32b4e7ebf11        debian:7            "ping google.com"   2 seconds ago       Up 1 seconds                            boring_nobel
172.17.0.8      f7d36f2b8e85        debian:7            "ping google.com"   12 seconds ago      Up 11 seconds                           jolly_turing
```
