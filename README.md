#!/bin/bash

# Update the package repositories and install necessary dependencies
sudo yum -y update
sudo yum -y install ruby wget python-pip

# Download and install the AWS CodeDeploy agent
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto

# Install AWS CLI
sudo pip install awscli
