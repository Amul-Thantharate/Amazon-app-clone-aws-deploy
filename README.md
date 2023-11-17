# Deploying Amazon Clone App in Aws Using Terraform and Jenkins Pipeline 


## Introduction 

This project is about deploying a react app in aws using terraform and jenkins pipeline.

## Prerequisites 

- AWS Account 
- Terraform 
- Jenkins 
- Docker
- SonarQube 
- Trivi 

## Steps 

- Go to aws account and create a new user with admin access and download the credentials file. 
- Install AWS cli and configure it with the credentials file. 
- Create a new ssh key pair in aws and download the private key.
- Download and install terraform. 
- Clone the repository 
- Go to the JENKINS-TF folder and run the following commands 
``` terraform fmt
    terraform init
    terraform plan
    terraform apply --auto-approve 
```
- New Ec2 Instance will be created with jenkins installed in it. 
- And jenkins and sonarqube will be running in the background. 

```
    To get the password of jenkins run the following command 
    sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

- Go to the jenkins url and login with the password. 
- Install the suggested plugins and create a new admin user.
