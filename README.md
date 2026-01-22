# azure-application-gateway-waf-iis
Secure Hosting of IIS Websites on Azure using Application Gateway, WAF, and Azure SQL Database
# Azure Secure IIS Hosting with Application Gateway, WAF & SQL Database

## 📌 Overview
This repository contains a Proof of Concept (POC) for securely hosting multiple IIS websites on a Windows Server Virtual Machine in Microsoft Azure.

The architecture uses **Azure Application Gateway with Web Application Firewall (WAF)** to manage traffic, enforce HTTPS, and restrict access exclusively to an office network. One website functions as a data entry application storing data in **Azure SQL Database**, while the second website is a normal IIS informational site.

---

## 🧩 Use Case
- Host multiple IIS websites on a single Windows Server VM
- Secure traffic using Azure Application Gateway + WAF
- Enable HTTPS (SSL)
- Restrict access to office network only
- Store application data securely in Azure SQL Database

---

## 🏗️ Architecture
Office Network / Internet
|
v
Azure Application Gateway (WAF v2)
|
v
Windows Server VM (IIS)
| |
Data Entry App Normal Website
|
v
Azure SQL Database

---

## 🛠️ Azure Services Used

- Azure Resource Group
- Azure Virtual Network (VNet)
- Azure Application Gateway (WAF v2)
- Windows Server 2022 Virtual Machine
- IIS Web Server
- Azure SQL Database
- Azure DNS / Custom Domains
- SSL Certificates

---

## 🔐 Security Features

- Web Application Firewall (OWASP rules)
- HTTPS (SSL termination at Application Gateway)
- No public access to VM or SQL Database
- Office IP–only access using WAF custom rules
- Restricted RDP access

---


---

## 🧪 Testing Performed

| Test Case | Result |
|----------|--------|
| Office network access | ✅ Allowed |
| External network access | ❌ Blocked |
| HTTPS enforcement | ✅ Working |
| SQL data insertion | ✅ Successful |
| WAF attack simulation | ✅ Blocked |

---

## 🚀 Outcome

- Successfully deployed two IIS websites in Azure
- Secured application using enterprise-grade architecture
- Implemented real-world Azure networking and security best practices

---

## 🔮 Future Enhancements

- Azure Bastion for secure RDP access
- Private Endpoint for Azure SQL Database
- Autoscaling for Application Gateway
- Azure Monitor & Log Analytics integration

---

## 👤 Author

**Sameeksha Y S**  
Azure | Cloud | DevOps Enthusiast  

---

## 📄 License
This project is for learning and demonstration purposes.





