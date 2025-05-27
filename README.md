<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>

# Organizing Workstations and Servers in Active Directory

## Platform and Tools Used
- TryHackMe Platform
- Virtual Machine
- Microsoft Active Directory

## Objective 
This project aims to demonstrates how to properly organize computer accounts in an Active Directory (AD) environment by creating and managing **Organizational Units (OUs)**. The goal is to separate machines by role—**Workstations and Servers**—to enable better policy application, security, and management.
___

 ## Steps Performed

 ###  Step 1: Identify Machines in "Computers"
- Review the default **Computers** container.
- Noted servers, user PCs, and laptops lumped together.
![Screenshot 2025-05-26 174245](https://github.com/user-attachments/assets/550493bc-cd0d-4772-a31d-3c39f988f25e)

### Step 2: Create Two New OUs Under the THM container 

![Screenshot 2025-05-26 175505](https://github.com/user-attachments/assets/9fae1c63-b794-4d06-ae69-5f8bf22aefb4)

 - Created a new OU named ‘Workstations'.
    
![Screenshot 2025-05-26 180023](https://github.com/user-attachments/assets/319b3917-ab01-4091-83a9-3a3f3947ed49)

- Created a new OU named 'Servers'.
  
![Screenshot 2025-05-26 180201](https://github.com/user-attachments/assets/df0c72ef-17f9-4f08-a22d-62dc2d9270f1)

- Verify the new OUs created are showing under the THM container:

 ![Screenshot 2025-05-26 180303](https://github.com/user-attachments/assets/eaf2b5d8-db1e-46c5-a401-7259a3d225c9)

 ### Step 3: Move Machines to Appropriate OUs

 - Moved personal laptops and user desktops to the Workstations OU.
![Screenshot 2025-05-26 182746](https://github.com/user-attachments/assets/c4392757-6ac7-40d8-8b39-5dbf87010a18)

- Moved service-related machines (like file or print servers) to the Servers OU.
![Screenshot 2025-05-26 183143](https://github.com/user-attachments/assets/3a9e9d23-d180-4ffd-8504-e072fcda9e49)

- Verify that all machines are now placed in their appropriate OUs.
 ![Screenshot 2025-05-26 183742](https://github.com/user-attachments/assets/39743646-8f44-4856-96b7-8022522e321c)![Screenshot 2025-05-26 183806](https://github.com/user-attachments/assets/35909d2d-859a-4839-949e-d218e831c3f5)
___

## Result 

- All AD-joined computers are now grouped by function.
- The environment is cleaner and better prepared for role-specific Group Policies.
- Ensures that future device additions follow a structured OU model.


