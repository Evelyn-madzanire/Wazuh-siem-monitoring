# 🛡️ Wazuh SIEM Monitoring – Homelab Project

This repository showcases my Wazuh SIEM (Security Information and Event Management) setup in a homelab environment.  
It demonstrates installation, configuration, agent deployment, threat detection, and log analysis using Wazuh Manager, Dashboard, and Agents.

---

## 🚀 Project Overview

This lab simulates a real-world SIEM environment and allows practicing SOC analyst skills. It includes:

- Installing Wazuh Manager and Dashboard on Ubuntu Server  
- Deploying Windows and Linux agents  
- Monitoring endpoints for security events  
- Detecting threats with Wazuh modules  
- Analyzing logs and alerts  

---

## 🔧 Features

### 1. Wazuh Installation
- Installed Wazuh Manager on Ubuntu Server  
- Set up Wazuh Dashboard for monitoring  
- Verified system services and manager status  

```bash
sudo apt update && sudo apt upgrade -y
curl -sO https://packages.wazuh.com/4.x/install.sh
sudo bash install.sh
sudo systemctl enable --now wazuh-manager
sudo systemctl enable --now wazuh-indexer
sudo systemctl enable --now wazuh-dashboard
