docker-redis
============

Redis Docker image

## Build Image

If you prefer to build the image instead of pulling from the public docker registry

    sudo docker login
    cd docker-redis

Build docker redis image (replace rudijs with <your-name> if you built your own docker image)

    sudo docker build -t rudijs/redis .

Review the new image

    sudo docker images
    
## Pull the image (if you did not build your own)

    sudo docker pull rudijs/docker-redis
    
## Run a redis container

Run the redis container (replace rudijs with <your-name> if you built your own docker image)

    sudo docker run -d -p 6379:6379 -name redis rudijs/redis

Check the status

    sudo docker ps -a
    sudo docker logs redis
