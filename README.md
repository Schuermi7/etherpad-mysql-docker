etherpad-docker
===============

This is a docker-compose File which you can use to deploy your own Etherpad-Lite https://github.com/ether/etherpad-lite.
(All of these instructions are made as root.)

To run Etherpad on port 9001, run:

`docker run -d -p 9001:9001 leibnitius/etherpad-docker`

To run Etherpad on port 80, run:

`docker run -d -p 80:9001 leibnitius/etherpad-docker`

To edit the Etherpad settings.json, it is necessary to clone the Git repository:

`git clone git://github.com/Schuermi7/etherpad-mysql-docker.git && cd etherpad-mysql-docker`

Then edit the settings.json to your liking, change your Database settings in the docker-compose.yml und run:

`docker-compose up` or `docker-compose up -d` to start it detached.
