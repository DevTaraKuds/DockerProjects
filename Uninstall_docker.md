# Uninstalling Docker on Kali Linux VM

Before deleting docker first delete images, containers, volumes etc using any of the following commands:

To delete all the docker container
```
docker rm -f (docker ps -a | awk '{print$1}')
````

To delete all the images
```
docker rmi -f $(docker images -a -q)
````

To delete all containers including its volumes
````
docker rm -vf $(docker ps -a -q)
````
Uninstall Docker
````
dpkg -l | grep -i docker
sudo apt-get purge -y docker-engine docker docker.io docker-ce docker-ce-cli
sudo apt-get autoremove -y --purge docker-engine docker docker.io docker-ce
````
