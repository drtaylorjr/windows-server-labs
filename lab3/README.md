# 🧪 Lab 3 – Simulate Group-Based Permission Planning (Active Directory)

## 🖥️ Lab Environment
- **Platform:** Azure VM (Windows Server 2022)
- **Role:** Domain Controller (AD DS Installed)
- **Domain Name:** `corp.local`
- **Tool Used:** Active Directory Users and Computers (ADUC)

---

## ✅ Objectives
- Create a new Organizational Unit (OU) for `Corp`
- Create Users and Groups inside the OU
- Assign users to appropriate security groups
- Simulate basic permission planning logic (via group membership)

---

## 📝 Steps Completed

| Task                           | Status        |
| ------------------------------ | ------------- |
| AD DS Installed                | ✅            |
| Domain Promoted (`corp.local`) | ✅            |
| ADUC Opened                    | ✅            |
| OUs Created (`_Corp > Users`)  | ✅            |
| Users Created                  | ✅            |
| Groups Created                 | ✅            |
| Users Assigned to Groups       | ✅            |
| Password Policy Viewed         | ✅ (optional) |
| Screenshots Taken              | ✅ (10 total) |

---

## 🧾 Notes

- **OU Naming:** Used underscore prefix (`_Corp`) to force sorting to the top
- **Usernames Used:** `John.Doe`, `Jane.Doe`, etc.
- **Groups Created:** `HR_Users`, `IT_Staff`, `Sales_Team`
- **Assignments:** Users were added to relevant groups simulating department-based access control

---

## 📸 Screenshots

> 📂 Screenshots saved in the `/screenshots/lab3/` folder  
> Naming convention used: `lab3_step1_aduc_opened.png`, `lab3_step2_create_ou.png`, etc.

---

## 🧠 Reflection

This lab demonstrated how to:
- Use OUs to logically organize directory objects
- Use groups to simulate permission assignments
- Practice foundational group-based access control (GBAC)

> This simulates how real help desk or junior sysadmin roles manage users and groups for access and compliance.

---



