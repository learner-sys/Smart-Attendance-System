# Architecture Overview
![aws](https://github.com/learner-sys/Smart-Attendance-System/assets/143533864/64c6e3b4-09c0-40c5-83d2-353cb2499c01)

Smart Attendance strategically harnesses a suite of AWS services including:
- Amazon Route 53: to create and manage the public DNS records.
- Amazon CloudFront: content delivery and better performance of web interface.
- AWS WAF: help protect your system.
- VPC: a virtual private cloud isolated network with our defined resources.
- Amazon S3: Store the captured images of attendees for backups records.
- AWS Lambda: function to trigger the processing of images stored in S3 buckets.
- Amazon Rekognition: for image processing and face recognition .
- Elastic Load Balancer: distribute incoming traffic across multiple instances
- Auto Scaling Groups: automatically scale EC2 instances based on the load
- DynamoDB: Store attendance records in a scalable database solution.
- Amazon EC2 instances: to set up cameras in classrooms for capturing images every 5 minutes.

</br> 
</br> 
These services collectively form the backbone of a highly available, scalable, and secure system. The architecture is established within a single AWS region, meticulously structured across two availability zones (AZs). This setup ensures fault tolerance and high availability, minimizing downtime risks by redundantly deploying resources across multiple physical locations.
Within the VPC, each AZ hosts a pair of subnets - a public subnet and a private subnet. The public subnet is equipped with NAT Gateway, Network Access Control Lists (NACLs), and security groups, facilitating controlled access to external resources and ensuring robust network security.
