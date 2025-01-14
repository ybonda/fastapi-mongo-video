# fastapi-mongo-video

## Explanation

[https://velocity.tech/blog/asynchronous-video-streaming-in-python-with-fastapi-and-mongodbs-gridfs](https://velocity.tech/blog/asynchronous-video-streaming-in-python-with-fastapi-and-mongodbs-gridfs)


## Run in Docker Compose
```shell
docker-compose -f docker_compose.yml up
```
## Run in Minikube
```shell
minikube start
minikube addons enable kong
minikube tunnel
```
```shell
cd fastapi-mongo-video/k8s
helm template . --values values.yaml | kubectl apply -f -
```

## Run in Velocity
```shell
cd fastapi-mongo-video/k8s
helm template . --values velocity-values.yml | veloctl env create -f -
```
