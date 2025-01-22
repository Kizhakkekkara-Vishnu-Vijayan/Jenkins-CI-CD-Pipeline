## Docker installation
Login into Jenkins EC2 Instance.

---
![Docker-1](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Docker-1.png) 

---
Run the following commands:
```
sudo apt update
sudo snap install aws-cli --classic
sudo su
```

---
![Docker-2](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Docker-2.png) 

Command to set the docker repository and repository key
```
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```

Command to install docker engine and docker cli
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```
Command to check the docker status
> Systemctl status docker

---
![Docker-3](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Docker-3.png) 

Since our Jenkins server is going to run all the docker commands, we need to add jenkins user into docker group. So that Jenkins server can run all the docker commands

Command to add jenkins user into docker group
> usermod -a -G docker jenkins

---
![Docker-4](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Docker-4.png) 

After that reboot the Jenkins server
> reboot