# 🛡️ Recovering Active Directory After a Security Incident

When identity falls, everything falls with it.

This project simulates a real-world Active Directory compromise and documents the full incident response lifecycle from detection and investigation to containment and secure recovery.

---

## 🧠 Scenario Overview

You are a security engineer responding to a compromised domain environment  
The mission is to identify malicious activity, determine scope, preserve evidence and restore trust in the environment.

---

## 🔍 Phase 1 Log and Identity Investigation

### Step 1: Identify Suspicious Group Activity

What event ID is logged when a user is removed from a universal security group?

 <img width="1435" height="362" alt="Recovering Active Directory Project Question 1 " src="https://github.com/user-attachments/assets/ec38837f-16d2-4463-970a-1b1162b75ce7" />


Finding  
Event ID 4757

<img width="1429" height="798" alt="Recovering Active Directory Project answer 1 " src="https://github.com/user-attachments/assets/0638f99c-7231-482e-9830-8d262324787a" />


---

### Step 2: Identify the Malicious User

What is the email address of the user, evil.guy? 

 <img width="1331" height="123" alt="Recovering Active Directory Project Question 2" src="https://github.com/user-attachments/assets/ba30e913-85e0-4ed3-92eb-b00d39ab10e1" />


Finding  
hack@crypto

 <img width="992" height="589" alt="Recovering Active Directory Project answer 2" src="https://github.com/user-attachments/assets/6fb4fe36-1490-4a82-9433-a33ef4d080f2" />


---

### Step 3 Confirm Log Visibility and Monitoring

What utility in Windows displays and keeps track of system events?

 <img width="1410" height="108" alt="Recovering Active Directory Project Question 3" src="https://github.com/user-attachments/assets/10cc30df-04e7-4bdb-ad65-2b0d2f1a802d" />


Finding  
Event Viewer


🧬 Phase 3 Recovery and Containment Preparation
Step 5: Backup and Evidence Preservation

What type of backups does Windows Server Backup support
<img width="1422" height="136" alt="Recovering Active Directory Project Question 5" src="https://github.com/user-attachments/assets/17d7e615-d85f-4591-b9a9-e566f3c0ff6d" />
Finding
Both one-time and incremental backups
<img width="1910" height="767" alt="Recovering Active Directory Project answer 5" src="https://github.com/user-attachments/assets/02e91623-027b-41eb-ab52-cffade7c4094" />
Step 6: Compromise Response Strategy

What is the correct order of actions when recovering a compromised Active Directory environment?

 <img width="1521" height="130" alt="Recovering Active Directory Project Question 6" src="https://github.com/user-attachments/assets/ac050b7d-02f6-4bf9-ab76-5d851631ec68" />


Finding
Prepare a cybersecurity policy and a disaster recovery plan
Take a backup of the compromised domain controller
Reset admin account passwords
Track group policy object changes
Forward logs to SIEM

 <img width="1485" height="329" alt="Recovering Active Directory Project answer 6" src="https://github.com/user-attachments/assets/172b930b-a7a0-4f25-ae52-5592631481f7" />

Step 7: Advanced Attack Awareness

What type of attack allows attackers to impersonate a domain controller and replicate domain data.

 <img width="1501" height="145" alt="Recovering Active Directory Project Question 7" src="https://github.com/user-attachments/assets/4808c07e-5113-4e29-a264-cc4acb408b1b" />


Finding
DCSync attack

<img width="1485" height="169" alt="Recovering Active Directory Project answer 7" src="https://github.com/user-attachments/assets/a26c95ca-b457-4a70-bb22-f206a2a336a2" />


Prevention includes monitoring replication permissions and disabling compromised accounts immediately.

 <img width="1306" height="758" alt="Recovering Active Directory Project answer 8" src="https://github.com/user-attachments/assets/34fba26b-2594-4313-aae3-a2a12cb8d1f8" />


🚀 Key Defensive Actions Taken

Look for compromised accounts and reset credentials

Change Kerberos service account password

Reset passwords of all administrative accounts

Reset computer machine passwords using Reset-ComputerMachinePassword

Reset the domain controller password to prevent Silver Ticket abuse

Perform malware analysis on domain controllers

Check for persistence mechanisms using the task scheduler via taskschd.msc

🧪 Tools and Technologies

Windows Server
Active Directory
Event Viewer
PowerShell
PowerView
Windows Server Backup
SIEM

🧠 Skills Demonstrated

Active Directory forensics
Identity threat detection
Enterprise incident response
Secure recovery operations
Domain hardening and containment
Advanced attack awareness

🙌 Credits

Built through hands-on Active Directory security and blue team incident response training.

