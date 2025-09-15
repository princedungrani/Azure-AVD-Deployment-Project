# Azure-AVD-Deployment-Project
# Azure Virtual Desktop (AVD) Deployment with Active Directory Integration  

## 📌 Project Overview  
This project demonstrates the deployment of a **secure and scalable Azure Virtual Desktop (AVD) environment** with an integrated Active Directory Domain Controller, profile management, and application delivery using MSIX.  

The solution provides centralized identity management, seamless app access, and persistent user profiles, simulating a real-world enterprise cloud desktop environment.  

---

## 🎯 Objectives  
- Deploy and configure **Domain Controller and Host Pools**.  
- Configure **Active Directory + Entra ID sync** for identity management.  
- Implement **FSLogix profile containers** for persistent user profiles.  
- Package and deploy applications with **MSIX App Attach**.  
- Secure access with **Multi-Factor Authentication (MFA)**.  
- Validate deployment using **Remote Desktop client and Web client**.  

---

## 🏗️ Architecture  
- **Domain Controller VM** – Windows Server 2019 with AD DS.  
- **User & Group Configuration** – Synced AD groups (cpoUsers) with Entra ID.  
- **Storage Account & File Share** – FSLogix profile containers with role-based access.  
- **Custom Image VM** – Windows 10/11 multi-session with Microsoft 365 Apps, FSLogix configured, sysprepped into a reusable image.  
- **Host Pool** – Pooled session hosts joined to AD.  
- **App Groups** – Desktop and Remote Apps (Word, Paint, MSIX packaged apps like XML Notepad).  
- **Testing** – MFA-enabled login, remote client access, profile persistence, and app delivery validation.  

---

## ⚙️ Requirements  
- Use `<StudentName>-S25P` as a prefix for resources.  
- Use assigned IP address ranges for VNet and subnets.  
- Consistent Azure region for deployment.  
- Video presentation length: **7–10 minutes** with webcam + audio.  

---

## ✅ Deliverables  
1. **Infrastructure Setup** – Resource groups, VNets, AD DS, Entra ID Sync.  
2. **Storage & FSLogix** – File share with proper roles and FSLogix containers.  
3. **Custom Image** – Multi-session VM sysprepped into an image.  
4. **Host Pool & App Groups** – Desktop + Remote apps deployed.  
5. **Testing** – MFA, Remote Desktop Client, Web Client, app functionality, and profile persistence.  

---


