## Bastion Host

- A Bastion Host is a public EC2 instance used to securely access private EC2 servers inside a VPC.
- It acts as a jump server between the internet and private instances.
- Keeps private EC2 instances hidden from internet

### Architecture Flow

        Laptop: → Bastion Host → Private EC2
----

## Create Bastion Host EC2 instance: 

 1. Click Launch Instances
 
 2. Name as  **bastion_host**
 
 3. AMI as **Ubuntu**
 
 4. Instance type- **t3.micro**
 
 5. Key Pair as required one
 
 6. Configure Network settings
    - Choose Security Group which has SSH access
    - VPC - **(aws-project-prod-vpc)**
    - Auto assign public IP- **Enable**
 
 7. Give Launch Instance
---

<img width="1110" height="238" alt="image" src="https://github.com/user-attachments/assets/e99f7c21-0a39-4cdd-9c4d-dabebaa3eab5" />

------

## Adding .pem File to the Bastion Host

- This makes us to securely connect from Bastion Host to the EC2 instances in the private subnet.

- Instead of copying .pem, we can use our local machine’s key through the Bastion Host. **Use SSH Agent Forwarding** is the best recommended method. 

- Copying .pem to Bastion Host increases security risk because the private key gets stored on another server.

**Note** - For learning purpose, here scp is used to copy .pem key to bastion host which should not do in real work.

------
 1. Via SCP .pem key is copied to bastion_host (public ip) from local machine
 
 2. SSH into bastion_host server

<img width="925" height="137" alt="ssh bastion host" src="https://github.com/user-attachments/assets/ebe5ed82-2619-4030-b3d5-1e3fa8e159a2" />

-----
 3. From there, SSH into private ip of EC2 instance

<img width="530" height="62" alt="ssh privateip" src="https://github.com/user-attachments/assets/799fdb89-ef17-454f-8815-179a7354adb8" />

-----

4. Here, a index.html file created to deploy.

5.  Run the Server by using **python3 -m http.server 8000**

<img width="543" height="58" alt="indexhtml" src="https://github.com/user-attachments/assets/95ba1753-57b1-4ba3-816d-7565d40c389b" />

------
