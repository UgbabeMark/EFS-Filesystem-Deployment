# EFS Filesystem Deployment

  This project demonstrates the creation and configuration of a shared file system using Amazon Elastic File System (EFS) on AWS. 

  EFS provides a scalable, highly available, and cost-effective solution for storing and sharing data across multiple EC2 instances.

# ![Enrollment](Images/efs.png)

# Resources Utilized

  EFS Filesystem: An Elastic File System is established to furnish scalable and shared storage across multiple EC2 instances.

  Security Group for EFS: A security group is devised to regulate the ingress and egress traffic for the EFS.

  EC2 Instances: Two EC2 instances are provisioned to access the shared EFS filesystem.

# Benefits of EFS:

  **Scalability:** EFS automatically scales storage capacity to meet your application's needs.

  **Durability:** Data is replicated across multiple Availability Zones for high availability and data protection.

  **Performance:** EFS provides consistent performance for concurrent access from multiple EC2 instances.

  **Cost-Effectiveness:** You only pay for the storage you use, making EFS a cost-efficient solution.


# Setup Instructions:

# 1. Create a Security Group for EFS:

  Create a security group to control the inbound and outbound traffic for the EFS. 

  Configure the security group rules as per your requirements.

# 2. Launch EC2 Instances:

  Launch two EC2 instances in different availability zones.

  Ensure that the instances are associated with the security group created for EFS.

# 3. Create an EFS Filesystem:

  Create an Elastic File System (EFS) filesystem. 

  Configure the filesystem settings, such as performance mode and throughput capacity.

# 4. Mount EFS on EC2 Instances:

  Mount the EFS filesystem on each EC2 instance to enable shared access to the storage. Configure the mount options and permissions as required.

# 5. Test the Shared Filesystem:

  Create files and directories on the mounted EFS filesystem from one EC2 instance and verify that they are accessible from the other EC2 instance. 

