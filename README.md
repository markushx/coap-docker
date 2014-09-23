coap-docker
===========

A Dockerfile with lots of CoAP implementations.

The built image is available at https://registry.hub.docker.com/u/markushx/coap/ . Feel free to modify and sent me your pull requests

Using the Image
===============

Start the image in interactive mode using using

`docker run -i -t -p 5683:5683/udp markushx/coap-docker`

This command binds your local UDP port for CoAP (5683)  to the docker instance.

Start any CoAP application, i.e. Californium:

    cd Californium/run
    java -jar cf-server-0.18.7-final.jar

Now you can access the CoAP server: `coap://127.0.0.1`


