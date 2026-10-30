# Week 1 Project: Cybersecurity Lab Setup

## Project Overview
This project sets up a virtual cybersecurity lab using Oracle VirtualBox and Kali Linux on a 10.0.0.0/24 NAT Network.

## Screenshots & Explanations

### 1. VirtualBox Network Adapter Configuration
This shows the Kali Linux VM attached to the custom NAT Network.
![Network Adapter](Screenshot%202026-10-30%20112912.png)

### 2. VM System Settings
This confirms the VM has 2048 MB of Base Memory, 2 processors, and the correct disk attached.
![System Settings](Screenshot%202026-10-30%20113746.png)

### 3. Kali Linux Desktop
Proof of a successful boot into the Kali Linux graphical interface.
![Kali Desktop](Screenshot%202026-10-30%20181943.png)

### 4. IP Configuration and Internet Test
The terminal shows eth0 is UP with the static IP 10.0.0.2/24. The ping google.com command shows 0% packet loss.
![IP and Ping Test](Screenshot_20261030-081647.png)

### 5. Virtual Machine Snapshot
A baseline snapshot named "full submission" was taken to save the clean state of the lab.
![Snapshot Manager](Screenshot_20261030-173017.png)

## Troubleshooting Experience
*Issue:* After setting the static IP, the Kali VM lost internet connectivity.
*Solution:* I used the nmcli command to disable the DAD timeout and restarted the connection.
