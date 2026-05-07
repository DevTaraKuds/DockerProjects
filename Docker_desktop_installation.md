<img width="1240" height="618" alt="Screenshot 2026-05-07 040422" src="https://github.com/user-attachments/assets/0acb355d-8dbf-4ec7-a359-4964da970d60" />

------------------------------------------------------------------------------------------------------------------------------------------------------------

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
Add docker to a group - Permission setting
````
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
