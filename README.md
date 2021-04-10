# flask-hello-world
Simple flask app in a docker container.

## Build instructions
1. `wget https://github.com/gliderlabs/docker-alpine/raw/2bfe6510ee31d86cfeb2f37587f4cf866f28ffbc/versions/library-3.8/x86_64/rootfs.tar.xz`
1. `docker build -t registry.infra.fogops.io/<your user/repo here>/flaskhelloworld .`
1. `docker push registry.infra.fogops.io/<your user/repo here>/flaskhelloworld`

## Run instructions
`docker run -d --rm -e  APP_NAME=blue -p 5000:5000 sbwise/flaskhelloworld:0.1.5`
