<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Launching VPC Resources

**Project Link:** [View Project](https://nextwork.ai/projects/8f49d756-9e51-58c0-856a-e71e54f064ab)

**Author:** Ahmed Umar Rehman  
**Email:** ahmedumar475@gmail.com

---

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8f49d756-9e51-58c0-856a-e71e54f064ab_8ee57662)

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is a logically isolated virtual network in AWS, and it is useful because it lets you securely control your AWS resources, networking, and traffic.

### How I used Amazon VPC in this project

I used Amazon VPC to create a secure virtual network, configure subnets and routing, and deploy EC2 resources within it.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was how many different AWS networking components work together to make a VPC secure and functional.

### This project took me...

This project took me 1 hour

## Setting Up Direct VM Access

Directly accessing a virtual machine means connecting to and controlling the VM remotely, usually through SSH or RDP.


### SSH is a key method for directly accessing a VM

SSH traffic means secure remote communication used to connect to and control a server, typically through port 22.

### To enable direct access, I set up key pairs

Key pairs are a public key and private key used to securely authenticate and access an EC2 instance.

A private key's file format means the format used to store the private key; my private key's file format was .pem because I selected RSA.

## Launching a public server

I had to change my EC2 instance's networking settings by placing it in the NextWork VPC and selecting the NextWork Public Subnet and Public Security Group.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8f49d756-9e51-58c0-856a-e71e54f064ab_88727bef)

## Launching a private server

My private server has its own dedicated security group because it allows me to control and restrict exactly what traffic can access the private server.

My private server's security group's source is the security group of my public server, which means only traffic from the public server is allowed to access the private server.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8f49d756-9e51-58c0-856a-e71e54f064ab_4a9e8014)

## Speeding up VPC creation

I used an alternative way to set up an Amazon VPC! This time, I used the VPC creation wizard to create the VPC and its networking components together.

A VPC resource map is a visual diagram that shows your VPC's resources and how they are connected to each other.

My new VPC has a CIDR block of 10.0.0.0/16. It is possible for my new VPC to have the same IPv4 CIDR block as my existing VPC because separate VPCs can use overlapping IP ranges as long as they are not directly connected through peering or other networking connections.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8f49d756-9e51-58c0-856a-e71e54f064ab_1cbb1b88)

## Speeding up VPC creation

### Tips for using the VPC resource map

When determining the number of public subnets in my VPC, I only had two options: 1 or 2. This was because the VPC wizard creates public subnets based on the number of Availability Zones selected.

The setup page also offered to create NAT gateways, which are services that allow resources in a private subnet to access the internet without allowing internet connections directly into them.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8f49d756-9e51-58c0-856a-e71e54f064ab_8ee57662)

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/8f49d756-9e51-58c0-856a-e71e54f064ab)*
