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

# port mapping
docker run -p80:3000 dvpxl/my-example
container exposes 80 maps to container's 3000

# volume mapping
docker run -it -v $(pwd):/container/path
