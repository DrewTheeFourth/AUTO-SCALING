# AUTO-SCALING - AUTOMATED DEPLOYMENT AND MANAGEMENT OF NGINX SERVERS IN THE CLOUD
ABOUT AUTO SCALING

EC2 Auto Scaling is a feature of AWS that automatically adjusts the number of Amazon EC2 instances in a group based on the demand for your application. It ensures that the right number of instances are running to handle the load, helping to maintain application availability and reduce costs.

Key Benefits of EC2 Auto Scaling:
Improved Availability: Auto Scaling ensures that your application always has the right amount of capacity to handle incoming traffic. It replaces unhealthy instances and maintains the number of instances you've set, ensuring availability.
Automatic Scaling: Based on scaling policies, EC2 Auto Scaling automatically adds or removes instances in response to demand, ensuring efficient resource usage and cost savings during off-peak times.
Cost-effective: You only pay for the resources you use. Auto-scaling helps minimize costs by running fewer instances when demand is low and scaling up automatically when needed.
Fault Tolerance: It continuously monitors the health of EC2 instances and replaces unhealthy instances automatically, enhancing the resilience of your application.
Easily Scalable: Auto Scaling allows you to quickly scale your infrastructure to meet demand, handling unpredictable traffic spikes without manual intervention.



PROJECT OVERVIEW

In this project, I provisioned an EC2 instance within a private subnet in a custom VPC. I then configured an Auto Scaling Group (ASG) to ensure scalability and high availability. I also deployed an Application Load Balancer (ALB) with defined target groups and successfully integrated it with the ASG. To optimize performance, I implemented Target Tracking scaling policies, setting the average vCPU utilization threshold at 30% to automatically manage scaling based on demand. 

The detailed steps for completing this project are outlined below:

Created a VPC with three public and private subnets.
Provisioned an EC2 instance within the private subnet and configured it with a user data script to automate the installation and maintenance of Nginx servers, ensuring continuous operation without manual intervention.
Configured and deployed an Auto Scaling Group (ASG).
Deployed an Application Load Balancer (ALB) with fully provisioned target groups to distribute incoming traffic efficiently across EC2 instances and attached it to the Auto Scaling Group.
Configured Target Tracking scaling policies within the Auto Scaling Group to maintain an average vCPU utilization threshold of 30%, enabling automatic scaling based on workload demand.



CHALLENGES ENCOUNTERED

While setting up the instance in the private subnet, I encountered challenges with SSH access. I determined that creating a bastion host was necessary to establish a secure connection, enabling SSH access to the private instance.



AWS RESOURCES UTILIZED

VPC: Utilized a VPC to create a secure and isolated network environment for deploying cloud resources, ensuring controlled access and segmentation. 
EC2: Deployed EC2 instances to host applications and services, providing scalable compute capacity within the cloud. 
Auto Scaling Groups: Implemented Auto Scaling Groups to automatically adjust the number of instances based on demand, ensuring high availability and optimal resource utilization.
Application Load Balancer: Deployed an application load balancer to efficiently distribute incoming traffic across multiple instances, enhancing application performance and reliability.



TECHNOLOGIES EMPLOYED

The use of Al tools in this project have been instrumental, they include ChatGPT, Perplexity and Google Gemini . I resorted to YouTube and Stack Overflow to figure out some complexities in this project.
