# Deployment of Java Application using Docker

This project consists of building and deploying the VProfile web application, 
developed by [hkhcoder](https://github.com/hkhcoder/vprofile-project) using Docker 
and Docker Compose.

The application was developed in Java, using JDK 11 and MySQL 8.

## Initial Settings: AWS EC2 Instance

To build and deploy the application, I launched an EC2 instance in AWS with the 
following specifications:

* Name: `build-vprofile-docker`

* AMI: `Ubuntu Server 24.04 LTS`

* Type: `t2.micro`

* RSA Key-pair generated as a `.pem` file

* Security group: Inbound rule

 - Type: All traffic

 - Source: My IP

I ran `sudo apt update` once inside the EC2 instance and checked the specifications 
using `cat /etc/os-release`:

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

## Install Docker Engine

I followed the steps to install Docker Engine for Ubuntu, as mentioned in the 
[Docker documentation page](https://docs.docker.com/engine/install/), using the 
`apt` repository.

The final step is verifying the installation process by running `docker run hello-world`:

```
$ sudo docker run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/
```
