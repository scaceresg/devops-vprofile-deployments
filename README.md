# DevOps deployment of Java Application using Docker

This project consists of building and deploying the VProfile web application, 
developed by [hkhcoder](https://github.com/hkhcoder/vprofile-project) using Docker and Docker Compose.

The application was developed in Java, using JDK 11 and MySQL 8.

## Initial Settings: AWS EC2 Instance

To build and deploy the application, I launched an EC2 instance in AWS with the following specifications:

* Name: `build-vprofile-docker`

* AMI: `Ubuntu Server 24.04 LTS`

* Type: `t2.micro`

* RSA Key-pair generated as a `.pem` file

I ran `sudo apt update` once inside the EC2 instance and check the specifications using `cat /etc/os-release`:

```
$ cat /etc/os-release
PRETTY_NAME="Ubuntu 24.04 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo
```

## 
