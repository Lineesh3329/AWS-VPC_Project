## Auto Scaling Group

- Auto Scaling Group is an AWS service that automatically manages EC2 instances by launching new servers when traffic increases and removing extra servers when traffic decreases.
-  It helps applications stay available, scalable, and cost-efficient without manual intervention.
------
## ASG Creation

  1. Go to EC2 Dashboard ---> **Auto scaling Groups**

  2. Click Create Auto Scaling Groups

  3. Click **Create Launch Template**
  
  4. Configuring Launch Template 

        - Name: **aws_project_prod**
      
        - AMI: choose **Ubuntu**
      
        - Instance Type: **t3.micro**
      
        - Key Pair: **Select required one** 

  5. Configure Network Settings as like below ( Inbound rules : Allow HTTP (8000) / SSH (22) ) 

<img width="875" height="448" alt="netwok asg" src="https://github.com/user-attachments/assets/b506a314-9a93-4c26-95e9-0e85f1cf5bd0" />

---

<img width="882" height="377" alt="netwrk2asg" src="https://github.com/user-attachments/assets/1cc2cce6-703f-47c3-86b3-47a6afdbec34" />

----
 
  6. Click **Launch Template**

  7. Configure Auto Scaling Groups

      - Choose created Lanuch Template.

      - Choose **Instance Launch Option**.
    
-------
<img width="856" height="414" alt="templateasgnetwork" src="https://github.com/user-attachments/assets/cf50a5da-7a6d-416e-9bcc-5ae70d7b2934" />

---
  8.  Configuring group size and scaling EC2 instance upto 4
 
<img width="835" height="390" alt="grpsize" src="https://github.com/user-attachments/assets/2e95e61b-b009-46dd-943c-57d2d19bc216" />

----
  9.  Click Create Auto Scaling Groups
      
  10.  Verify its created and showing Instances as 2.
     
<img width="1314" height="274" alt="asgcraeated" src="https://github.com/user-attachments/assets/7c345478-936f-47df-bc83-c3869a4590ea" />

----
  11. Check that two EC2 instances created.

<img width="1121" height="212" alt="asg running" src="https://github.com/user-attachments/assets/93710788-ac5f-44fa-831a-9c8e03bd512c" />

----
