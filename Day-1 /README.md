# 📅 Day 01 - Linux User Setup with Non-Interactive Shell

## 📌 Topics Covered
- Linux User Management  
- Creating Users in Linux  
- Interactive vs Non-Interactive Shell  

---

## 🧠 What I Learned

In Linux, users can be created with different types of shells depending on their purpose.  

- **Interactive Shell** → Allows login and command execution (e.g., `/bin/bash`)  
- **Non-Interactive Shell** → Prevents login access, used for service or system accounts (e.g., `/sbin/nologin` or `/bin/false`)  

Non-interactive shells are important for security, especially when creating users that should not have login access.

---

## ⚙️ Commands Practiced

### 🔹 Create a User with Non-Interactive Shell
```bash
sudo useradd -s /sbin/nologin username

##🔍 Explanation
useradd → Command to create a new user
-s → Specifies the login shell
/sbin/nologin → Disables interactive login
