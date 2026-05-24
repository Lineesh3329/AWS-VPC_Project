## VPC Creation

1. Open Amazon VPC Console

2. Click Create VPC

3. Select:
   VPC and more

4. Enter VPC name

5. Keep default **IPv4** CIDR block- Default one ( 10.0.0.0/16 )
   
6. Select:
   - **2** Availability Zones
   - **2** Public Subnets
   - **2** Private Subnets

7. Keep default subnet CIDR blocks
   OR
   customize subnet CIDR blocks

8. Select:
   **1** NAT Gateway per Availability Zone

9. Select:
    None- not as S3 Gateway Endpoint

10. Disable:
    Enable DNS hostnames

11. Click:
    Create VPC
----

<img width="365" height="535" alt="vpcsetupsuccess" src="https://github.com/user-attachments/assets/ee0f7356-ba94-447e-a6ee-f2de79a1760c" />

----------
### Resource Map

<img width="1083" height="374" alt="resourcemap" src="https://github.com/user-attachments/assets/2c923f12-1dab-4ff4-8083-6600f03830b0" />

------------
### Verify created VPC

<img width="1169" height="215" alt="vpcs" src="https://github.com/user-attachments/assets/346fb8d4-13f3-4937-8a57-d497898dfc3a" />

---
