# Selenium grid on docker

Docker-compose file to start selenium grid with Chrome and Firefox browser nodes

For more info about running selenium in docker see [https://github.com/SeleniumHQ/docker-selenium](https://github.com/SeleniumHQ/docker-selenium)

## Prerequisites

1. [Docker engine](https://docs.docker.com/engine/installation/)

2. [Docker compose](https://docs.docker.com/compose/install/)

## Installation

    $ git clone https://github.com/lopezs/selenium-grid-docker.git mygrid

## Usage

Start the selenium grid hub service:
    
    $ cd mygrid
    $ docker-compose up -d

Your test runners will connect to ```hostmachine_ip:4444```


If you want to add more nodes:

    $ docker-compose scale nodefirefox=10 nodechrome=10

