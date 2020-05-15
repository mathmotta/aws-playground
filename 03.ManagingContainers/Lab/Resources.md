# Resources

This week we started to dive deeper into orchestration and built the foundation for using Amazon Elastic Container Service. The additional readings continue with those themes and help prepare you to better understand orchestration, orchestration tools, and Amazon ECS. 

 

 

## Orchestration

 

If you have a handful of containers running a few applications, it's not that difficult to manage the deployment and maintenance of your containers. However, if you have thousands of containers running hundreds of services, management gets much more complex.

 

When you're operating at scale, automated container orchestration - the deployment, management, scaling, networking, and availability of your containers - becomes essential. Container orchestration is all about managing the lifecycles of containers, especially in larger, production-scale environments.

 

Read more about container orchestration with ECS and Fargate:  https://www.youtube.com/watch?v=cpqvIEgngcY&list=PLhr1KZpdzukfWFTsOD_WynnY2-e8TY8fH&index=5

 

 

## What is Amazon ECS

 

Amazon ECS is a highly scalable, high performance container management service that supports Docker containers and allows you to easily run applications on a cluster of Amazon EC2 instances. 

 

Amazon ECS eliminates the need for you to install, operate, and scale your own container management tools and infrastructure. With simple API calls, you can launch and stop container-enabled applications, query the state of your cluster, and leverage many familiar AWS features like Security Groups, Elastic Load Balancing, EBS volumes and IAM roles. 

 

For more information on Amazon ECS, check out the FAQs:  https://aws.amazon.com/ecs/faqs/

 

 

## Introduction to Amazon ECS

 

Amazon Elastic Container Service integrates with AWS IAM for permissions. Amazon ECS uses an IAM Role to create resources on your behalf using role-based access, and Tasks also have IAM Roles associated with them to allow processes running in the task to make API calls to AWS services. 

 

Click here to learn more about how Amazon ECS integrates with AWS IAM:  https://docs.aws.amazon.com/AmazonECS/latest/userguide/security_iam_service-with-iam.html

 

Amazon Elastic Container Service allows you to take advantage of multiple EC2 pricing options. One of those options is to run EC2 spot instances as a part of your cluster. To learn more about using Amazon ECS or AWS Fargate with Spot Instances click here: 

https://aws.amazon.com/ec2/spot/containers-for-less/get-started/

https://aws.amazon.com/blogs/aws/aws-fargate-spot-now-generally-available/

 

As a best practice, you shouldn’t bake your secrets directly into your docker images. Instead consider using a service like AWS Secrets Manager to store and access secrets in a secure and programmatic way.

 

To learn more about AWS Secrets Manager click here: 

https://aws.amazon.com/secrets-manager/

 

 

## Scheduling and Task Placement with Amazon ECS

 

Amazon ECS provides flexible scheduling and placement capabilities for your tasks and containers. You can choose to manually run your tasks, run them on a cron-like schedule, use a custom scheduler, or run tasks using an ECS service scheduler. 

 

ECS also allows you to use task placement constraints and task placement strategies to customize how ECS places your tasks. 

 

For more information, see the following links on scheduling and placing:

https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html

 

https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement.html