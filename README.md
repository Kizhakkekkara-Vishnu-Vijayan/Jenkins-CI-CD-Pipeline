## Overview
This project demonstrates an end-to-end CI/CD pipeline built using Jenkins to automate the build, test, code quality analysis, containerization, and deployment processes for a Java-based application.

## Project Description
The Project demonstrates how a Jenkins CI/CD pipeline integrates several tools and technologies, including Maven, SonarQube, Docker, and AWS services like ECR and ECS, to provide a robust, scalable, and automated deployment solution.

### Technologies and Tools Used

- Jenkins: Continuous integration and delivery automation.
- Maven: Build automation and dependency management.
- SonarQube: Static code analysis and quality gate enforcement.
- Docker: Containerization of the application.
- Amazon ECR: Storage for container images.
- Amazon ECS: Deployment and orchestration of containerized applications.

### Prerequisites
Before setting up and running the pipeline, ensure you have the following installed and configured on your system:

1. Git: For cloning the repository and version control.
2. Jenkins: Installed and configured with necessary plugins like Maven, Docker, and SonarQube.
3. Maven: For building and testing the Java application.
4. SonarQube: Set up locally or via a cloud instance for code analysis.
5. Docker: Installed and running to build and manage containers.
6. AWS CLI: Configured with appropriate IAM permissions for ECR and ECS operations.
7. Java JDK: Required to compile and run the Java application and to run Maven commands.

### What Developers do:
- Developers collaboratively write and commit code changes to a centralized version control system, such as GitHub.
- Their primary responsibility is to write, build, and test the code locally, ensuring it functions correctly before pushing the changes to GitHub. 
---
 ![Project flow diagram](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Developer.png)

### What DevOps Engineer do:
- DevOps engineers key responsibilities include, configuring and maintaining infrastructure, monitoring system performance, and ensuring the reliability, scalability, and security of applications.
- DevOps engineers streamline the software development lifecycle by automating processes, managing CI/CD pipelines, and ensuring seamless integration between development and operations
---
![Project flow diagram](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/DevOps.png)

## Project flow diagram
---
![Project flow diagram](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-SS-ALL/Flow-diagram.png)

---
## Project Flow execution steps :
1. Login to AWS Account
2. Jenkins Installation

[Jenkins Installation](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-Installation/Jenkins-Setup.md)
```
├───Jenkins-Installation
│   ├───Jenkins-Setup.md
```

3. Jenkins plugins 

[Jenkins Plugins Installation](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-Plugins/Jenkins-Plugins.md)
```
├───Jenkins-Plugins
│   ├───Jenkins-Plugins.md
```

4. SonarQube Installation

[SonarQube Installation](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/SonarQube/SonarQube-Installation.md)
```
├───SonarQube
│   ├───SonarQube-Installation.md
```

5. Docker Installation

[Docker Installation](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Docker/Docker-Installation.md)
```
├───Docker
│   ├───Docker-Installation.md
```

6. AWS IAM

[IAM Setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/AWS/AWS-IAM.md)
```
├───AWS
│   ├───AWS-IAM.md
```
7. AWS ECR

[ECR Setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/AWS/AWS-ECR.md)
```
├───AWS
│   ├───AWS-ECR.md
```

8. AWS ECS

[ECS Setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/AWS/AWS-ECS.md)
```
├───AWS
│   ├───AWS-ECS.md
```

9. Jenkins Pipeline

[Pipeline Setup](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Jenkins-Pipeline/Pipeline-Setup.md)
```
├───Jenkins-Pipeline
│   ├───Pipeline-setup.md
```

10. SonarQube Output

[SonarQube Output](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/SonarQube/SonarQube-Output.md)
```
├───SonarQube
│   ├───SonarQube-Output.md
```

11. CI/CD Output validation

[CI/CD Output validation](https://github.com/Kizhakkekkara-Vishnu-Vijayan/Jenkins-CI-CD-Pipeline/blob/master/Output-Validation.md)
```
├───Output-validation.md
```
