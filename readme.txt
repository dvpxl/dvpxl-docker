Work in progress ...

# create tag of image using build command
docker build -t dvpxl/my-example .

```
REPOSITORY    TAG         IMAGE ID       CREATED          SIZE
<none>        <none>      595861477de2   14 seconds ago   90.6MB

Changes to:

REPOSITORY    TAG         IMAGE ID       CREATED          SIZE
dvpxl         my-example  595861477de2   14 seconds ago   90.6MB
```

# run 
docker run -it dvpxl/my-example cmd

# attach to already running container 
docker exec -it container_id /bin/sh

# port mapping
docker run -p80:3000 dvpxl/my-example
container exposes 80 maps to container's 3000

# volume mapping
docker run -it -v $(pwd):/container/path

# remove all images (this still did not relinquish space), see next.
sudo docker images prune -a

# remove all images and relinquish space (will relinqiush space)
sudo docker system prune

# start a stopped container
sudo docker start container_id

# list all containers
sudo docker ps -a

# commit already running container
docker commit container_id

