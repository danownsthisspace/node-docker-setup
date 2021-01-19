This is an example of an basic docker setup for a node api

### Build image:

    docker build -t node-api:v1 .

## Start container

    docker run --name node-app -p 3000:3000 -v $(pwd):/app node-api:v1

## To automatically remove container when stopped add --rm before starting container

    docker run --rm --name node-app -p 3000:3000 -v $(pwd):/app node-api:v1

## Stop running container using

    docker stop node-app

## List all docker images:

    docker image ls -a

## List all docker containers:

    docker ps -a

## To delete a stopped container

    docker rm {container id / container name}

## To delete an image

    docker rmi {image id}




