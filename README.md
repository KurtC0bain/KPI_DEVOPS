# KPI_DEVOPS

1. To build the Docker image
```
  docker build . -t prom3tei/devops-docker-node-app
```
2. To see if image is listed by Docker
```
  docker images
```
3. Push an image or a repository to a registry
```
  docker push prom3tei/devops-docker-node-app
```
4. Run the container in detached mode, leaving the container running in the background. Use ```-m``` and ```--cpus``` flags to limit mamory and cpu
```
  docker run -m 100m --cpus="2" -p 80 -d prom3tei/devops-docker-node-app
```
5. To test an app, get the port of app that Docker mapped using
```
  docker ps
```
6. Then run the app on localhost:80
