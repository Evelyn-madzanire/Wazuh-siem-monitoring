- # 🛡️ Wazuh SIEM Monitoring – Homelab Project

This project showcases my Wazuh SIEM (Security Information and Event Management) setup in a homelab environment. It covers installation, configuration, agent deployment, threat detection, and log analysis using Wazuh Manager, Wazuh Dashboard, and Wazuh Agents.

---

## 🚀 Project Overview
This repository documents how I built and configured a Wazuh-based monitoring environment to practice SOC analyst skills. It includes:

- Installing the Wazuh Manager and Dashboard
- Deploying Windows and Linux agents
- Monitoring endpoints for security events
- Detecting threats with Wazuh modules
- Analyzing logs and alerts

---

## 🏗️ Lab Architecture

            ┌────────────────────┐
            │  Wazuh Dashboard   │
            └─────────┬──────────┘
                      │
            ┌─────────▼──────────┐
            │   Wazuh Manager    │
            │   (Ubuntu Server)  │
            └─────────┬──────────┘
                      │
     ┌────────────────┼────────────────┐
     │                │                │





---

## 🔧 Features

### 1. Wazuh Installation
- Installed Wazuh Manager on Ubuntu Server
- Set up Wazuh Dashboard for monitoring
- Verified system services and manager status

```bash
# Example commands used for installation
sudo apt update && sudo apt upgrade -y
curl -sO https://packages.wazuh.com/4.x/install.sh
sudo bash install.sh
sudo systemctl enable --now wazuh-manager
sudo systemctl enable --now wazuh-dashboard

