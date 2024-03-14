#!/bin/bash

# Update the package repositories and install necessary dependencies
sudo yum -y update
sudo yum -y install ruby wget python-pip

# Download and install the AWS CodeDeploy agent
cd /home/ec2-user
