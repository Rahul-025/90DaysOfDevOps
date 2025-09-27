# Week 2: Linux System Administration & Automation

Welcome to **Week 2 of the 90 Days of DevOps - 2025 Edition!**
This week was all about **Linux system administration & automation 🚀**.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

I explored **users, groups, permissions, logs, processes, volumes, and shell scripting**. Here’s my **hands-on journey with solutions 👇**

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🚀 Project: DevOps Linux Server Monitoring & Automation

### I worked on real-world server admin tasks like:
- Managing users & SSH access
- Setting file permissions
- Doing log analysis with grep, awk & sed
- Handling volumes & disk usage
- Monitoring processes
- Automating backups with shell scripting

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 📌 Tasks & Solutions
### 1️⃣ User & Group Management

### Commands:

#### Create user
sudo useradd devops_user  

#### Create group
sudo groupadd devops_team  

#### Add user to group
sudo usermod -aG devops_team devops_user  

#### Set password
sudo passwd devops_user  

#### Give sudo access
echo "devops_user ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/devops_user  

#### Restrict SSH for some users
sudo vim /etc/ssh/sshd_config

DenyUsers test_user

#### Restart ssh
sudo systemctl restart ssh
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### ✅ Successfully created devops_user with sudo rights and secured SSH.
