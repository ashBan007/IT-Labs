# Lab 08: Active Directory - OU, User & Group Management

## Objective
Create Organizational Units (OUs), create user accounts, and manage security groups in Active Directory.

## Tools Used
- Windows Server 2022
- Active Directory Users and Computers

## Steps Performed

### 1. Created Organizational Units (OUs)
- Opened **Active Directory Users and Computers**.
- Right-clicked on `lab.local` domain.
- Created 3 new OUs: **Sales**, **HR**, and **IT**.

### 2. Created User Accounts
- Right-clicked on the **Sales** OU.
- Created 4 new users:
  - Asgar Ali
  - Imran Mir
  - Ishak mahmud
  - Md Shadi
- Configured passwords and set "Password never expires" for lab purposes.

### 3. Created Security Group
- Right-clicked on the **Sales** OU.
- Created a new Security Group named **Sales-Team**.

### 4. Added Users to Group
- Opened the properties of **Sales-Team**.
- Went to the **Members** tab.
- Added all 4 users to the group.

## Results
- Successfully structured the AD environment by separating users into OUs.
- Created user accounts and assigned them to a specific team (Group).
- This setup allows applying Group Policies (GPO) to specific departments and managing file share permissions easily.

## What I Learned
- The difference between an OU (Organizational Unit) and a Group.
- How to create and manage user accounts.
- Best practices for organizing users based on departments.
- How to add users to security groups for permission management.

## Screenshots
Screenshots are in the `screenshots/` folder.