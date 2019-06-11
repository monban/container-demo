# container-demo
Build a docker image

    docker build -t {{image-name}} .

Run a simple container in the background

    docker run -d {{image-name}}

Stop and remove a running container

    docker rm -f {{container name or id}}

Create a new running container and forward a port

    docker run -d -p {{host-port}}:{{container-port}} {{image-name}}

Create a new running container mounting a local directory as a volume

    docker run -d -v {{directory}}:{{volume}} {{image-name}}
