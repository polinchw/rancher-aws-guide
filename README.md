# rancher-aws-guide
This repo will serve as a guide for setting up a usable Rancher infrastructure on AWS.

## Contents
- AWS Cloud Formation
- Run a Rancher Server

## AWS Cloud Formation
Rancher can control many different servers running docker within your business.  If you're running your business on AWS
you can set up an AWS VPC for your Rancher infrastucture to run on using AWS Cloud Formation.  This repo will help you set up your AWS VPC for Rancher to run it's docker hosts on:

https://github.com/polinchw/rancher-aws-cloudformation

## Run a Rancher Server
Once you have your AWC VPC running you'll want to install the Rancher server on it along with SSL so it can be accessed securly over the internet.  This repo will help you install the Rancher server on the RancherAdmin EC2 instance that was created with the cloud formation script in the previous step

https://github.com/polinchw/rancher-ssl
