# 📅 Day 02 - Temporary User Setup with Expiry

## 📌 Topics Covered
- Linux User Management  
- Setting User Expiry Date  
- Account Lifecycle Management  

---

## 🧠 What I Learned

In Linux, we can create users with an **expiry date**, which means the account will automatically be disabled after a specific date.

This is useful when:
- Giving temporary access to users  
- Managing contract-based employees  
- Improving system security by avoiding unused accounts  

---

## ⚙️ Commands Practiced

### 🔹 Create User with Expiry Date
```bash
sudo useradd -e YYYY-MM-DD username
