# Docker Desktop

To install docker desktop on Kali Linux, the following commands are used. 

#### Installing Docker dependencies
````
sudo apt-get update 
sudo apt install docker.io docker-compose
````

#### Confirm installation
```
docker version
docker-compose version
````
#### Run docker demo
```
sudo  docker run hello-world
````

#### Set group permissions
````
Add docker to a group - Permission setting
sudo usermode -aG docker $USER
````

#### reboot system
````
sudo reboot
````

#### Verify setting
````
sudo nano /etc/group
````

#### test any docker command without sudo
````
docker ps -a
````
