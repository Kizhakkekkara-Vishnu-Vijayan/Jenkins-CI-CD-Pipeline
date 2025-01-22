## Creating IAM User 

---
![IAM-1](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-1.png) 

Attach policy of __AmazonEC2ContainerRegistryFullAccess__, so that jenkins instance can upload the docker images into Amazon ECR.

---
![IAM-2](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-2.png) 

Attach policy of __AmazonECS_FullAccess__, so that jenkins instance can deploy the latest docker container of Amazon ECR into Amazon ECS.

---
![IAM-3](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-3.png) 

---
![IAM-4](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-4.png) 

Now create access key for jenkins user

---
![IAM-5](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-5.png) 

---
![IAM-6](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-6.png) 

---
![IAM-7](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-7.png) 

---
After creating Access key, store the IAM user Access key in Jenkins server credentials tab

---
![IAM-8](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-8.png) 

---
![IAM-9](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/IAM-9.png) 