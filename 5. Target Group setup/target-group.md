# Target Group
- A Target Group is an AWS component, routes traffic from the Application Load Balancer (ALB) to healthy EC2 instances using health checks.
- Target Group acts like a bridge between ALB and EC2.

            User Request
                 ↓
            Application Load Balancer
                 ↓
            Target Group
                 ↓
            EC2 Server

## Creating Target Group

  1. Goto EC2 → Target Groups → Create

  2. Target type: **Instances**
    
  3. Target Group Name : **aws-project-prod**
    
  4. Protocol: **HTTP**
    
  5. Port: **8000**
    
  6. VPC: Created vpc- **aws_project_prod_vpc**
    
  7. Health Check:

         Path: /
         Protocol: HTTP
    
  8. Register Targets - Created EC2 Instances

------
<img width="919" height="477" alt="2target group" src="https://github.com/user-attachments/assets/6da14d3c-2592-4924-a7e7-ca5716e282ae" />

------
 9. Verify created Target group

<img width="1135" height="167" alt="created tg" src="https://github.com/user-attachments/assets/031d32c2-0f77-4448-be4c-53cd176a902e" />

---
