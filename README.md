# VProfile Multi-Tier Deployment (DevOps Hands-On Project)

This project showcases my hands-on DevOps setup where I built a **complete multi-tier environment** for a Simple Java Web Application using **Vagrant**, **VirtualBox**, and **Linux**.  
The entire stack was deployed manually first and then fully automated using shell provisioning.

---

## 📘 Project Overview

This setup replicates a realistic production-like environment where each major service runs on its own virtual machine.  
It helped me understand how backend services integrate and how to automate Infrastructure as Code on a local system.

### **Key Goals**
- Provision 5 VMs using **Vagrant + VirtualBox**  
- Configure database, cache, message broker, app server, and web server  
- Deploy a Java application on **Tomcat**  
- Route traffic through **Nginx reverse proxy**  
- Validate full end-to-end workflow (DB → App → Cache → Queue)  
- Automate provisioning using Bash scripts  

---

## 🧱 Architecture

| Service | Role | VM Name | IP Address | OS |
|--------|------|----------|------------|-----|
| MySQL | Database | `db01` | 192.168.56.15 | CentOS 9 |
| Memcached | Caching Layer | `mc01` | 192.168.56.14 | CentOS 9 |
| RabbitMQ | Message Broker | `rmq01` | 192.168.56.13 | CentOS 9 |
| Tomcat | Application Server | `app01` | 192.168.56.12 | CentOS 9 |
| Nginx | Reverse Proxy / Web Layer | `web01` | 192.168.56.11 | Ubuntu 22.04 |

---

## ⚙️ Tools & Technologies

- **Vagrant** – VM provisioning  
- **VirtualBox** – Hypervisor  
- **Linux** (CentOS & Ubuntu)  
- **MariaDB / MySQL** – Database  
- **Memcached** – Caching  
- **RabbitMQ** – Messaging Queue  
- **Tomcat 10** – Java application server  
- **Nginx** – Web server + reverse proxy  
- **Maven** – Build Java WAR file  
- **Git & GitHub** – Version control  

---

# 📸 Screenshots – Full Deployment Walkthrough

Below are the screenshots demonstrating each major step of the project setup.

---

## 🖥️ 1. All Vagrant Machines (global-status)

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174011" src="https://github.com/user-attachments/assets/15ba6f53-4186-43a9-8df8-a53f7cc3d468" />

---

## 🧰 2. VirtualBox – All Machines Running

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174050" src="https://github.com/user-attachments/assets/d4d68dd1-a09e-4c7a-b3a4-9d3b0d43f09e" />

---

## 🧩 3. Hostname Automation – vagrant-hostmanager

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174210" src="https://github.com/user-attachments/assets/bccdc699-e02f-49b0-920a-dd602c37fea0" />

---

## 🚀 4. Tomcat Deployment (systemd + Java App)

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174427" src="https://github.com/user-attachments/assets/523911d2-6832-4a8f-9fd2-6f276d2f6783" />

---

## 🗄️ 5. MySQL Database Imported Successfully

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174657" src="https://github.com/user-attachments/assets/8e92e7ee-bace-4e60-8873-adbbd5b7ed5c" />

---

## 🔐 6. Application Login Page (via Nginx)

<img width="1919" height="1079" alt="Screenshot 2025-11-12 174949" src="https://github.com/user-attachments/assets/4c12e3e2-8591-4a64-8674-79ddac68862a" />

---

## 🏠 7. Application Dashboard

<img width="1919" height="1079" alt="Screenshot 2025-11-12 175004" src="https://github.com/user-attachments/assets/7cf36567-b630-436f-a5d1-2115889fd54b" />

---

## 📋 8. Users List – Dynamic Data from MySQL

<img width="1919" height="1079" alt="Screenshot 2025-11-12 175013" src="https://github.com/user-attachments/assets/8d41a421-cdcb-4c2d-823f-875b77ad9b2b" />

---

## 🐇 9. RabbitMQ Initiated – Connections, Channels, Queues

<img width="1919" height="1079" alt="Screenshot 2025-11-12 175049" src="https://github.com/user-attachments/assets/d24ff228-445d-452f-94c3-26529f60266a" />

---

## 📦 10. User Details – Data loaded from DB and inserted into Cache

<img width="1919" height="1079" alt="Screenshot 2025-11-12 175023" src="https://github.com/user-attachments/assets/f93e1003-e3af-47b1-856a-bd12a10398db" />

---

## ⚡ 11. Cached Response – Memcached Working

<img width="1919" height="1079" alt="Screenshot 2025-11-12 175032" src="https://github.com/user-attachments/assets/defd2b13-8a47-4300-b8e4-520b9e026748" />

---

# 🧾 Summary

This project demonstrates:

✔ Full-stack environment provisioning  
✔ Manual + automated setup  
✔ Understanding of multi-tier architecture  
✔ Hands-on Linux administration  
✔ Real-world integration across 5 services  
✔ Effective use of Infrastructure as Code  
✔ Service validation through actual UI & logs  

This was one of the most practical DevOps labs I've completed, and the screenshots above show every part of the environment working together as a functional system.
