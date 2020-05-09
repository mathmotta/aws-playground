# Lab 3 Goal

Deploying local is done. The challenge is now dealing with host configuration in AWS. We need to launch two containers on a host using Beanstalk and with one or more EC2's.

Host EC2's dont have nicely prepared volumes waiting to be used, we need to get seeded data on to those hosts. Best way to get shared data is to use .ebextensions

## Goals

1. Push images
2. Backup images to Amazon ECR
3. Setup a dockerrun.aws.json file
4. Prepare volume data for host using .ebextensions