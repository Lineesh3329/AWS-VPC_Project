# Load Balancer
- A Load Balancer is an AWS service that distributes incoming traffic across multiple EC2 servers to improve availability, scalability, and performance.
- Without Load Balancer cause Server overload, Slow performance, Downtime risk
- With Load Balancer Better performance, High availability, Fault tolerance
      
        1000 users
            ↓
        Load Balancer
         ↓    ↓    ↓
        EC2  EC2  EC2
-----

## Creating Load Balancer
  1. Go to EC2 --> Load Balancer
  
  2. Click Create Load Balancer

  3. Select **Application Load Balancer**
  
  4. Name: **aws-project-prod**
     
  5. Scheme: **Internet-facing**

  6. IP address type: **IPv4**

  7. Network Mapping
     - VPC: Choose created one **aws-project-prod-vpc**
     - Choose minimum two public AZ

<img width="1075" height="451" alt="albnetwork" src="https://github.com/user-attachments/assets/99aa47b5-ab09-4f83-b45f-a19e5ff161df" />

------
  8. Security Group: Inbound Rules: HTTP (80) → 0.0.0.0/0
  9. Listeners and Routing
     
              Listener: HTTP (Port 80)
              Default action: Forward to a Target Group
              Select created Target Group - aws-project-prod
      

<img width="1066" height="377" alt="22listeners" src="https://github.com/user-attachments/assets/9919ad1b-23ec-4a32-abb5-858a793ef134" />

----
  10. Click Create Load Balancer
    
  11. Verify created LB
<img width="1135" height="165" alt="lb" src="https://github.com/user-attachments/assets/8cf9f246-5a2c-4eda-af0f-a1a52bcb8422" />

-----

<img width="1101" height="302" alt="port80" src="https://github.com/user-attachments/assets/3c638396-74a6-4f89-be33-3a1ff83d0312" />

----
