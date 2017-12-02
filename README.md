# rancher-aws-guide
This repo will serve as a guide for setting up a usable Rancher infrastructure on AWS.

## Contents
- AWS Cloud Formation
- Rancher Server Access
- Rancher Access Control
- Create a Rancher Environment
- Set your Rancher Host Registration URL
- Docker Release Guide

## AWS Cloud Formation
Rancher can control many different servers running docker within your business.  If you're running your business on AWS
you can set up an AWS VPC for your Rancher infrastucture to run on using AWS Cloud Formation.  This repo will help you set up your AWS VPC for Rancher to run it's docker hosts on:

https://github.com/polinchw/rancher-aws-cloudformation  (return to this page after this step)

## Rancher Server Access

Point your browser to the public IP of the Rancher server and the Rancher UI will come up.

https://public-ip

![alt text](https://raw.githubusercontent.com/polinchw/rancher-ssl/master/images/rancher-startup.JPG)

## Rancher Access Control

Once your Rancher Server is up and running you should set up a means of authentication so that only you can access the service.

![alt text](https://raw.githubusercontent.com/polinchw/rancher-ssl/master/images/rancher-admin.JPG)

## Create a Rancher Environment

Create a Rancher enviroment in the Rancher UI.

![alt text](https://raw.githubusercontent.com/polinchw/rancher-aws-guide/master/images/rancher-env.JPG)

## Set your Rancher Host Registration URL

Set the your Rancher Host URL to the private IP of the Rancher server.  

![alt text](https://raw.githubusercontent.com/polinchw/rancher-aws-guide/master/images/rancher-hostreg.JPG)

Example http://10.0.1.106:8080

## Docker Release Guide
After your Rancher server is running you'll probably want to release your company's code using docker.  This guide shows how to 
build, tag, and release docker containers.  Even though Docker Machine is mentioned in this guide don't worry because Rancher basically is a fancy Docker Machine infrastructure.  So instead of creating a Docker Swarm with the repo's bash script you'd use Rancher to create a swarm.  

https://github.com/polinchw/docker-release-guide
