# KPI_DEVOPS

1. To build the Docker image
```
  docker build . -t prom3tei/devops-docker-node-app
```
2. To see if image is listed by Docker
```
  docker images
```
3. Run the container in detached mode, leaving the container running in the background. Use ```-m``` and ```--cpus``` flags to limit mamory and cpu
```
  docker run -m 100m --cpus="2" -p 14880:8080 -d prom3tei/devops-docker-node-app
```
4. To test an app, get the port of app that Docker mapped using
```
  docker ps
```
5. Then run the app on localhost:14880
