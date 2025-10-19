# AWS HIGH AVAILABILITY & DISASTER RECOVERY ARCHITECTURE
  -High Availability & Disaster Recovery Architecture with ELB Failover Simulation on AWS
 

# PROJECT OVERVIEW
  -This project demonstrates a **High Availability (HA)** and **Disaster Recovery (DR)** setup on AWS using a **multi-region architecture**
  The goal was to ensure that the application remains available even if one AWS region fails. 


#  AWS SERVICES USED
  1.**EC2** – Web servers deployed in multiple regions  
  2.**Elastic Load Balancer (ELB)** – Distributes incoming traffic  
  3.**Auto Scaling Group (ASG)** – Maintains instance health and scalability  
  4.**Route 53** – DNS failover and health checks


# ARCHITECTURE SUMMARY
  1.Two EC2 instances hosted in **Region A** and **Region B**
  2.Each region has its own **Elastic Load Balancer** 
  3.**Route 53** monitors health of Region A using DNS failover  
  4.When Region A fails, traffic automatically routes to **Region B** 
