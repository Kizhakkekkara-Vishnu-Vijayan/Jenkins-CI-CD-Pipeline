## Jenkins installation
- Launch an EC2 instance with following configurations:  
  - Provide a name for EC2 instance, like 'Jenkins-Server' 
  - Select the AMI as Ubuntu Server 24.04 LTS
  - Select Instance type as t3.small
  - Create a key pair
  - Create security group with SSH(22) from My IP, and Custom TCP(8080) from My IP

![Jenkins-Install-1](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-Install-1.png)
![Jenkins-Install-2](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-Install-2.png)

### Login into the Jenkins EC2 instance:
> ssh -i <path_of_.pem(key)> ubuntu@<public-IP>

- Run the following commands:
```
sudo -i

apt update

apt install openjdk-21-jdk -y

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

sudo apt-get update

sudo apt-get install jenkins
```
> ssh into EC2

![ssh-jenkins](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ssh-jenkins.png)
> java -version

![java-version](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/java-version.png)
> systemctl status jenkins

![Jenkins-status](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-status.png)

Now type the jenkins public IP Address along with port number 8080 to access jenkins server from browser.
![Jenkins-IP-Port](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-IP-Port.png)

To get the initial password for accessing jenkins, run the following command:
> cat /var/lib/jenkins/secrets/initialAdminPassword
![Jenkins-Password](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-Password.png)

Paste the Initial Admin Password here
![Jenkins-First-Login](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-First-Login.png)

Customize Jenkins
![Customize-Jenkins-1](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Customize-Jenkins-1.png)

Create Username and Password
![Uname-Passwd](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Uname-Passwd.png)

Default URL
![URL](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/URL.png)

Jenkins Dashboard
![Jenkins-Dashboard](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Jenkins-Dashboard.png)

Installing Maven Plugin
![Maven-Plugin](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Maven-Plugin.png)

Installing JDK Plugin
![JDK-Plugin](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/JDK-Plugin.png)