# VProfile Multi-Tier Deployment

This project showcases my hands-on DevOps setup where I built a **complete multi-tier environment** for the **VProfile web application** from scratch.  
The goal was to deploy and connect multiple services (database, cache, message broker, application server, and web server) across **five virtual machines** using **Vagrant**, **VirtualBox**, and **Linux automation**.

---

## 📘 Project Overview

This project simulates a real-world web application environment where each service runs on a separate virtual machine.  
It helped me understand how different layers of an application work together and how to automate infrastructure provisioning locally.

**Key Objectives:**
- Learn how to set up and automate a multi-tier application stack locally.  
- Understand how different backend services integrate together.  
- Practice Infrastructure as Code using **Vagrant**.  
- Gain end-to-end deployment experience similar to real DevOps workflows.

---

## 🧱 Architecture

| Service | Role | VM Name | IP Address | OS |
|----------|------|----------|-------------|----|
| MySQL | Database | `db01` | 192.168.56.15 | CentOS 9 |
| Memcached | Caching Service | `mc01` | 192.168.56.14 | CentOS 9 |
| RabbitMQ | Message Broker | `rmq01` | 192.168.56.13 | CentOS 9 |
| Tomcat 10 | Application Server | `app01` | 192.168.56.12 | CentOS 9 |
| Nginx | Load Balancer / Web Server | `web01` | 192.168.56.11 | Ubuntu 22.04 |

Each VM runs one service, making the setup modular and realistic for production-style environments.

---

## ⚙️ Tools and Technologies Used

- **Vagrant** – Automates creation and configuration of virtual machines  
- **Oracle VirtualBox** – Hypervisor for running the VMs  
- **Git & GitHub** – Version control and source management  
- **Linux (CentOS, Ubuntu)** – Base OS for each VM  
- **MySQL** – Database layer  
- **Memcached** – Cache layer  
- **RabbitMQ** – Message queuing service  
- **Apache Tomcat** – Application hosting  
- **Nginx** – Reverse proxy and load balancer  
- **Maven** – Java build tool for packaging the app  

---
