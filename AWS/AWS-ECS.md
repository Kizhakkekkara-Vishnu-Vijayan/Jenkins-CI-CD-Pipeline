## Creating ECS(Elastic Container Service)
Amazon ECS is a container orchestration platform similar to that of Kubernetes, but ECS is limited to AWS where as Kubernetes serves as a Multi-cloud deployment service, preventing Vendor-lock

ECS creation Steps

1. Create Cluster

---
![ECS-1](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-1.png)

---
![ECS-2](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-2.png)

---
![ECS-3](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-3.png) 

2. Create Task Definitions

![ECS-4](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-4.png)

---
![ECS-5](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-5.png)

---
![ECS-6](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-6.png) 

- Add __CloudWatchLogsFullAccess__ in ecsTaskExecutionRole which atomatically gets created when we create Task Definition.
- This cloudwatch logs will help us identify error which we may encounter while deploying our ECR container into ECS

---
![ECS-7](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-7.png) 

3. Create Service 

Service is used to manage Task of ECS cluster which can also be called as containers. So, Service can be used to manage the container.

Service creation steps

![ECS-8](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-8.png)

---
![ECS-9](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-9.png)

---
![ECS-10](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-10.png) 

![ECS-11](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-11.png)

---
![ECS-12](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-12.png)

---
![ECS-13](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-13.png) 

---
![ECS-14](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/ECS-14.png)