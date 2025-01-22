## SonarQube Setup 
- Launch an EC2 instance with following configurations:  
  - Provide a name for EC2 instance, like __Sonar-Server__ 
  - Select the AMI as __Ubuntu Server 24.04 LTS__
  - Select Instance type as __t3.medium__
  - Create a key pair
  - Create security group with __SSH - 22__ from My IP, __Custom TCP - 80__ from My IP and __Custom TCP - 80__ from Jenkins-Server security group.
---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-1.png)

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-2.png)

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-3.png)

Go to Advanced details and copy paste the following bash script configuration of [SonarQube-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/SonarQube/SonarQube-Setup.sh) in user data 


Once the EC2 Instance of Sonar-server is in active and running state, Login into the instance using browser and enter public IP address of SonarQube Server
Enter the username and password as admin
Remember to enter new credentials for the username and password

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-4.png)

Edit the security group of jenkins with __Custom TCP - 8080__ from Sonar-Server security group. So that the SonarQube server can provide the result to Jenkins server.

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-5.png) 

Go to Jenkins -> Manage Jenkins -> Tools, and add SonarQube Scanner 6.2.1 which we installed using Jenkins plugins.

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-6.png) 

Go to Jenkins -> Manage Jenkins -> System -> SonarQube servers -> check the Environment Variables 
---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-7.png) 
---

- To enable SonarQube server to access Jenkins server, we need to add SonarQube secret key in Jenkins server.
- Go to SonarQube server and click on My Account -> Security.
- Enter Name, type and expiry in days inside the General Token settings.
- Then click on generate.
- Copy the generated token.
- Paste the token in Jenkins, inside server authentication token 


---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-8.png) 

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-9.png) 

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-10.png) 

---
![Sonar-setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Sonar-11.png) 
