# 🛡️ Recovering Active Directory After a Security Incident

When identity falls, everything falls with it

This project simulates a real-world Active Directory compromise and documents the full incident response lifecycle from detection and investigation to containment and secure recovery

---

## 🧠 Scenario Overview

You are a security engineer responding to a compromised domain environment  
The mission is to identify malicious activity, determine scope, preserve evidence and restore trust in the environment

---

## 🔍 Phase 1 Log and Identity Investigation

### Step 1: Identify Suspicious Group Activity

What event ID is logged when a user is removed from a universal security group

 <img width="1435" height="362" alt="Recovering Active Directory Project Question 1 " src="https://github.com/user-attachments/assets/ec38837f-16d2-4463-970a-1b1162b75ce7" />


Finding  
Event ID 4757

<img width="1429" height="798" alt="Recovering Active Directory Project answer 1 " src="https://github.com/user-attachments/assets/0638f99c-7231-482e-9830-8d262324787a" />


---

### Step 2: Identify the Malicious User

What is the email address of the user evil.guy

 <img width="1331" height="123" alt="Recovering Active Directory Project Question 2" src="https://github.com/user-attachments/assets/ba30e913-85e0-4ed3-92eb-b00d39ab10e1" />


Finding  
hack@crypto

 <img width="992" height="589" alt="Recovering Active Directory Project answer 2" src="https://github.com/user-attachments/assets/6fb4fe36-1490-4a82-9433-a33ef4d080f2" />


---

### Step 3 Confirm Log Visibility and Monitoring

What utility in Windows displays and keeps track of system events

 <img width="1410" height="108" alt="Recovering Active Directory Project Question 3" src="https://github.com/user-attachments/assets/10cc30df-04e7-4bdb-ad65-2b0d2f1a802d" />


Finding  
Event Viewer

 <img width="1300" height="808" alt="Recovering Active Directory Project answer 3" src="https://github.com/user-attachments/assets/69903bd8-65a4-4124-9bc5-8dfae49bbe7d" />


---

## 🧭 Phase 2 Environment Reconnaissance

### Step 4 Domain Enumeration

How many machines exist in the domain
 
Command executed

```powershell
Get-NetComputer | Select Name
Finding
11 machines discovered




