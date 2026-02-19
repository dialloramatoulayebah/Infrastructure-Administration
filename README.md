# Infrastructure-Administration
# 🖥️ Infrastructure Administration – Hyper-V Virtualization Lab

## 📌 Project Overview

This project demonstrates the creation and management of a fully functional virtualized infrastructure using **Microsoft Hyper-V**.

The objective was to simulate real-world system administration tasks including:

- Virtual machine deployment  
- Storage provisioning and management  
- Checkpoint lifecycle control  
- Nested virtualization  
- Internal network isolation  

This lab was completed as part of my coursework in **IT Infrastructure Administration**.

---

## 🎯 Project Objectives

- Deploy a Windows Server 2022 virtual machine (Generation 2)
- Configure fixed memory (4GB) and 4 virtual processors
- Create and manage standard checkpoints
- Add and configure a fixed-size virtual disk (1GB)
- Initialize, partition, and format storage volumes
- Implement nested virtualization
- Deploy a sub-virtual machine inside the main VM
- Configure an internal virtual switch
- Validate configurations using checkpoint restoration

---

## 🏗️ Infrastructure Architecture

### 🔹 Main VM – TP6

| Component | Configuration |
|-----------|---------------|
| OS | Windows Server 2022 |
| Generation | 2 |
| Memory | 4GB (Fixed) |
| Virtual Processors | 4 |
| Main Disk | 40GB VHDX |
| Additional Disk | 1GB Fixed (P: Drive – NTFS) |

---

### 🔹 Nested VM – STP6

| Component | Configuration |
|-----------|---------------|
| Hosted Inside | TP6 |
| Memory | 1GB |
| Disk | 5GB |
| Feature | Hyper-V Nested Virtualization Enabled |

---

## 💾 Storage Configuration

A secondary virtual disk was added and configured as:

- **Type:** Fixed Size  
- **Capacity:** 1GB  
- **File System:** NTFS  
- **Drive Letter:** `P:`  
- **Volume Label:** `TP6_12`  
- **Validation File:** `file_12.txt`  

This demonstrates disk provisioning and volume management within a virtualized environment.

---

## 🔄 Checkpoint Strategy

Four standard checkpoints were created to secure each major stage of the configuration:

1. `CheckPoint1_12` – Initial VM configuration  
2. `CheckPoint2_12` – After disk addition and file creation  
3. `CheckPoint3_12` – After nested virtualization setup  
4. `CheckPoint4_12` – Final configuration with internal switch  

This strategy ensures safe rollback and configuration integrity.

---

## 🌐 Network Configuration

An **Internal Virtual Switch** was configured to:

- Allow communication between host and VM  
- Maintain network isolation  
- Simulate controlled enterprise networking environments  

---

## 🧠 Skills Demonstrated

- Hyper-V virtual machine deployment  
- Resource allocation and optimization  
- Virtual storage management  
- Checkpoint lifecycle management  
- Nested virtualization configuration  
- Internal network setup  
- Infrastructure rollback validation  

---

## 📷 Screenshots

This repository includes screenshots demonstrating:

- VM configuration settings  
- Checkpoint hierarchy  
- Disk Management (P: drive)  
- Nested VM deployment  
- Internal virtual switch setup  

---

## 🏆 Key Learning Outcomes

Through this project, I strengthened my understanding of:

- The role of a hypervisor in infrastructure management  
- Virtual resource allocation  
- Infrastructure scalability and flexibility  
- Backup and recovery strategies in enterprise IT  
- Network isolation within virtualized systems  

---

## 🚀 Why This Project Matters

This lab simulates real-world IT infrastructure scenarios commonly used in:

- Enterprise server environments  
- Virtual lab deployments  
- Cloud-ready infrastructures  
- System administration training  

It reflects practical, hands-on experience in virtualization and infrastructure management.

---

## 👩🏽‍💻 Author

**Ramatoulaye Diallo**  
IT Infrastructure & Systems Student  
Bilingual (English / French)  



