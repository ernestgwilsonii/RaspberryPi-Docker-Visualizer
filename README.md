# RaspberryPi-Docker-Visualizer
Raspberry Pi Docker Visualizer

```
###############################################################################
time docker pull alexellis2/visualizer-arm:latest

# Deploy
docker stack deploy -c docker-compose.yml vizualizer-stack
#docker stack rm vizualizer-stack

# Verify
docker stack ls
docker service ls | grep vizualizer-stack
docker service logs -f vizualizer-stack_vizualizer
###############################################################################
```