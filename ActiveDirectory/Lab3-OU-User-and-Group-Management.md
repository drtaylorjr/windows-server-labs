# Lab 3: OU, User, and Group Management in Active Directory

## Lab Objective
Set up Organizational Units (OUs), create user accounts, create security groups, and assign users to appropriate groups inside Active Directory using ADUC (Active Directory Users and Computers).

---

## Lab Environment
- **Platform:** Azure VM  
- **OS:** Windows Server 2022  
- **Role:** Domain Controller (AD DS Installed)  
- **Domain:** `corp.local`  
- **User:** Logged in as Domain Administrator  
- **Tools Used:** Active Directory Users and Computers (ADUC)

---

## Step-by-Step Instructions

### ✅ Step 1: Launch Active Directory Users and Computers (ADUC)
- Open **Server Manager**
- Click **Tools > Active Directory Users and Computers**
- Confirm the domain is visible (`corp.local`)

📸 **Screenshot 1:** ADUC console open on domain `corp.local`

---

### ✅ Step 2: Create Parent OU `_Corp`
- Right‑click the domain (`corp.local`)
- Select **New > Organizational Unit**
- Name it `_Corp`

📸 **Screenshot 2:** `_Corp` OU created under domain

---

### ✅ Step 3: Create Sub‑OUs `Users` and `Groups`
- Right‑click `_Corp` > **New > Organizational Unit**
- Name the first OU **Users**
- Repeat and create **Groups**

📸 **Screenshot 3:** OUs `Users` and `Groups` created under `_Corp`

---

### ✅ Step 4: Create New User Accounts
- Right‑click the **Users** OU > **New > User**
- Create the following accounts:

#### **John Doe**
- First Name: John  
- Last Name: Doe  
- Username: `jdoe`  
- Password: `P@ssword1`  
- Uncheck: *User must change password at next logon*

📸 **Screenshot 4:** John Doe account creation window

#### **Jane Doe**
- First Name: Jane  
- Last Name: Doe  
- Username: `jadoe`  
- Password: `P@ssword1`  
- Uncheck: *User must change password at next logon*

📸 **Screenshot 5:** Jane Doe account creation window

---

### ✅ Step 5: Create Security Groups
- Right‑click the **Groups** OU > **New > Group**
- Create the following:

#### **Accounting**
- Group Scope: Global  
- Group Type: Security  

#### **HR**
- Group Scope: Global  
- Group Type: Security  

📸 **Screenshot 6:** Accounting group created  
📸 **Screenshot 7:** HR group created

---

### ✅ Step 6: Add Users to Groups
- Right-click **Accounting** > **Properties > Members > Add**
  - Add: `jdoe`
- Right-click **HR** > **Properties > Members > Add**
  - Add: `jadoe`

📸 **Screenshot 8:** jdoe added to Accounting  
📸 **Screenshot 9:** jadoe added to HR

---

### ✅ Step 7: View Password Policy (Optional)
- Open **Group Policy Management**
- Expand:
  - `Forest: corp.local`
  - `Domains`
  - `corp.local`
- Right‑click **Default Domain Policy** > **Edit**
- Navigate:
  `Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy`

📸 **Screenshot 10:** Default Domain Password Policy displayed

---

## Completion Checklist

| Task                           | Status |
| ------------------------------ | ------ |
| AD DS Installed                | ✅ |
| Domain Promoted (`corp.local`) | ✅ |
| ADUC Opened                    | ✅ |
| OUs Created (`_Corp > Users`)  | ✅ |
| Users Created                  | ✅ |
| Groups Created                 | ✅ |
| Users Assigned to Groups       | ✅ |
| Password Policy Viewed         | ✅ (optional) |
| Screenshots Taken              | ✅ |

---

## Notes
- OU naming convention (`_Corp`) forces it to appear at the top for easier management.  
- Password complexity requirements enforced by default.  
- Group membership simulates real-world role-based access control.  

---


