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
🔹 Example
sudo useradd -s /sbin/nologin mariyam
🔹 Verify User
cat /etc/passwd | grep mariyam
🔍 Explanation
useradd → Command to create a new user
-s → Specifies the login shell
/sbin/nologin → Disables interactive login
📚 Use Cases
Service accounts (e.g., web servers, database users)
Automation scripts
System-level processes
🚀 Hands-on Practice
Created a user with restricted login access
Verified the assigned shell
Understood how non-interactive users improve security
🧪 Exercise

Create two users with a non-interactive shell:

sudo useradd -s /sbin/nologin user1
sudo useradd -s /sbin/nologin user2
✅ Verify
cat /etc/passwd | grep user1
cat /etc/passwd | grep user2
💡 Key Takeaway

Not all users need login access.
Using non-interactive shells improves system security and control.

🔥 Day 01 completed — consistency started!


---

If you want, next I can:
- Build your **Day-02 README (Linux commands + permissions + real examples)**
- Or help you make your repo look 🔥 with **badges + formatting + profile README**

Just tell me 👍


