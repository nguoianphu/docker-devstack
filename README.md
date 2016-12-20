# Docker DevStack image

[![Build Status](https://travis-ci.org/nguoianphu/docker-devstack.svg?branch=master)](https://travis-ci.org/nguoianphu/docker-devstack)
[![](https://images.microbadger.com/badges/image/nguoianphu/docker-devstack.svg)](http://microbadger.com/images/nguoianphu/docker-devstack "Get your own image badge on microbadger.com")


### Build

        docker build -t devstack .
        
### Run
        docker run -d -p 80:80 -p 5000:5000 --name my-devstack devstack
        
        # or
        docker run -d -p 80:80 -p 5000:5000 --name nguoianphu-devstack nguoianphu/docker-devstack
        
### When the script finishes executing, you should be able to access OpenStack endpoints, like so:

#### Horizon:
        http://DOCKER_IP/
#### Keystone:
        http://DOCKER_IP:5000/v2.0/
