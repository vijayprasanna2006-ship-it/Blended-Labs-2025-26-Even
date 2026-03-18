
# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : Prasanna V   
Reg no : 212223210018  
Date : 18/03/2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

## Workflow

1. Logged into AWS Console  
2. Opened EC2 Dashboard  
3. Reviewed existing instances  
4. Verified VPC and subnets  

### Launch Template Creation
5. Navigated to Launch Templates  
6. Clicked "Create Launch Template"  
7. Entered template name  
8. Selected Amazon Machine Image  
9. Chose instance type  
10. Configured key pair  
11. Attached security group  
12. Added user data script  
13. Created launch template  

### Auto Scaling Group Setup
14. Navigated to Auto Scaling Groups  
15. Clicked "Create Auto Scaling Group"  
16. Selected launch template  
17. Configured VPC and subnets  
18. Set desired capacity  
19. Set minimum capacity  
20. Set maximum capacity  
21. Enabled health checks  
22. Created Auto Scaling Group  

### Load Balancer Configuration
23. Navigated to Load Balancers  
24. Selected Application Load Balancer  
25. Configured load balancer name  
26. Selected internet-facing scheme  
27. Chose VPC and subnets  
28. Created target group  
29. Selected instance target type  
30. Configured health check path  
31. Registered EC2 instances  
32. Created load balancer  

### Integration
33. Attached ASG to target group  
34. Verified instance registration  
35. Enabled load balancing  

### Scaling Policy Setup
36. Opened CloudWatch service  
37. Created CPU utilization alarm  
38. Set threshold value  
39. Linked alarm to scaling policy  
40. Configured scale-out policy  
41. Configured scale-in policy  

### Testing and Validation
42. Generated traffic using browser/tool  
43. Observed request distribution  
44. Monitored instance scaling  
45. Verified high availability  
46. Tested fault tolerance  

---

## Output Screenshots 

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/e37c51b3-131d-490b-9996-81414a020182" />
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1eafd64a-d883-432c-b8d2-b6c19053081e" />
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/0dd34e8e-3035-45f1-ada0-2d564b6509cf" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
