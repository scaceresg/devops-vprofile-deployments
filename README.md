# Deploying a Java Application using Different Approaches

This project consists of building and deploying the VProfile web application, 
developed by [hkhcoder](https://github.com/devopshydclub/vprofile-project) using 
different deployment approaches.

The application is **`vprofile web application`** and is developed in Java
using JDK 11/8 and contains the following services:

![Image by Zudonu Osomudeya](https://miro.medium.com/v2/resize:fit:1189/1*cP0KJ_UOjHhUHCdxSDIsCw.png)
Image by Zudonu Osomudeya

* Web Service: NGINX

* Application Server: Tomcat

* SQL Database: MySQL 8

* DB Memory Caching: Memcached

* Broker/Queuing Agent: RabbitMQ

* Indexing/Search Service: ElasticSearch

I am performing this project as part of my learning process as a student of the
[DevOps Beginners to Advanced with Projects](https://www.udemy.com/course/decodingdevops/)
Udemy course.

The deployment approaches I used here are:

* Lift & Shift Migration

* Platform as a Service (PaaS): AWS Beanstalk & Amazon RDS

* [Docker Compose in AWS EC2 Instance](https://github.com/scaceresg/devops-vprofile-deployments/tree/07d28fb16c45171a737b610769fc50459f3770a8/docker-aws-ec2)

* CI Jenkins Pipeline

* Docker + CI/CD Jenkins Pipeline

* Docker + Kubernetes (EKS)

* Docker + EKS + CI/CD Jenkins Pipeline
