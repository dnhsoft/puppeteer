puppeteer docker image
====================

Docker image with Google Puppeteer installed

Example usage
--------------------

``` yaml
# docker-compose.yml
tests:
    image: dnhsoft/puppeteer:latest
    network_mode: host
    volumes:
      - "./src/tests:/app/"
    command: ["/bin/bash", "-c", "yarn install && while true; do sleep 10000; done"]
```
