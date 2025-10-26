# AWS HIGH AVAILABILITY & DISASTER RECOVERY ARCHITECTURE

High Availability & Disaster Recovery Architecture with ELB Failover Simulation on AWS
 

# PROJECT OVERVIEW
   
This project demonstrates a **High Availability (HA)** and **Disaster Recovery (DR)** setup on AWS using a **multi-region architecture**
  The goal was to ensure that the application remains available even if one AWS region fails. 


#  AWS SERVICES USED
 
-  **EC2**– Web servers deployed in multiple regions  
-  **Elastic Load Balancer (ELB)**– Distributes incoming traffic 
-  **Auto Scaling Group (ASG)**– Maintains instance health and scalability  
-  **Route 53**– DNS failover and health checks


# ARCHITECTURE SUMMARY

Two EC2 instances are hosted in Region A and Region B, each with its own Elastic Load Balancer (ELB). Route 53 monitors the health of Region A and manages DNS failover, ensuring that if Region A fails, 
   traffic is automatically redirected to Region B, maintaining high availability and disaster recovery.


# OUTCOME / RESULTS

-  **Zero Downtime:** The application remained available even when Region A was intentionally taken offline.  
-  **Automatic Failover:** Route 53 DNS failover successfully redirected traffic to Region B without manual intervention.  
-  **High Availability:** Multi-region EC2 setup with ELB and ASG ensured continuous service availability.  
-  **Scalability:** Auto Scaling Groups allowed the architecture to handle varying loads efficiently.  
-  **Disaster Recovery:** Demonstrated an effective strategy for disaster recovery across regions, minimizing business impact.

# ARCHITECTURE DIAGRAMS / SCREENSHOTS

**High Availability & Disaster Recovery setup**


<img width="997" height="747" alt="Screenshot 2025-10-24 095403" src="https://github.com/user-attachments/assets/ca90ba10-678b-431e-8bf7-28196839011d" />


**EC2 instances**


<img width="1907" height="843" alt="EC2-A" src="https://github.com/user-attachments/assets/52308d05-11fd-411d-8cc4-2ecb2eafbaf0" />    <img width="1902" height="842" alt="EC2-B" src="https://github.com/user-attachments/assets/9f10ba4c-f10d-48e4-a168-746ed110eacc" />


**Auto Scaling Group configuration**


<img width="1905" height="846" alt="myAutoscalinggroup-A" src="https://github.com/user-attachments/assets/d08d6686-f290-41b3-a3dd-5fbf421c86c0" />  <img width="1902" height="842" alt="MyAutoscalingG-B" src="https://github.com/user-attachments/assets/3cec62e7-3b89-42d5-a04b-cedf60cace37" />


**ELASTIC LOAD BALANCER (ELB) setup**


<img width="1902" height="802" alt="LB-A" src="https://github.com/user-attachments/assets/f0761e7b-2746-438d-bb92-7f00f8b11c07" />   <img width="1902" height="842" alt="LB-B" src="https://github.com/user-attachments/assets/dcbef59e-c5dc-4466-9011-c47f555de464" />


**ROUTE 53 HEALTH CHECK & FAILOVER**


<img width="1918" height="913" alt="route53" src="https://github.com/user-attachments/assets/aaba6e69-853b-43e0-8c07-4906cea60943" />


**application running in Region A**


<img width="753" height="848" alt="index html A" src="https://github.com/user-attachments/assets/477566e2-83a7-431f-a1a2-a29a34920019" />


**application running in Region B  after Route 53  triggered a DNS failover**


<img width="1911" height="907" alt="regionB" src="https://github.com/user-attachments/assets/0c884684-6090-4fb7-9db9-83de11e203cb" />











