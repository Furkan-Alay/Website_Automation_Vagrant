# 📄 Project Overview

This repository contains automation scripts for setting up virtual machines using **Vagrant**. You can easily deploy multiple VMs with predefined configurations and provisioning scripts.

---

## 📌 Requirements

- Install **Git Bash** terminal (recommended for Windows users)
- Install **Oracle VM VirtualBox**
- Install **Vagrant**

---

## 📥 How to Use

1. Clone this repository to your local machine (C: or F: drive recommended).
2. Use the Vagrantfiles located inside the `finance`, `ubuntu`, `centos` and other directories to create and manage virtual machines.
3. You can customize the VM configurations by editing the corresponding **Vagrantfile**.

---

## 📦 Vagrant Commands

```bash
vagrant up               # Start the VM based on the Vagrantfile configuration  
vagrant halt             # Stop the running VM  
vagrant destroy          # Remove the VM  
vagrant status           # Show the current status of the VM  
vagrant global-status    # Show the status of all Vagrant-managed VMs  
vagrant ssh              # Connect to the VM via SSH  
```
# 📂 Project Structure
### finance
Contains a Vagrantfile with provisioning scripts. It installs Apache Web Server and assigns a static IP address via the private network. You can access the web server through your browser using the configured static IP.

### financeIAC
Similar to the finance directory, but includes a provisioning script that fetches a pre-built web template and places it into the Apache server’s directory. You can customize the provisioning to deploy your own website automatically.

### wordpressIAC
Automates the installation of WordPress. Once the VM is up, you can access your WordPress site through the configured static IP.

### multiVM
Demonstrates how to manage multiple VMs using a single Vagrantfile. You can customize the VMs and resources as needed.

📌 Notes

All provisioning steps are handled within each Vagrantfile.

You can easily modify IP addresses, network settings, and provisioning scripts to suit your environment.

Great for practicing Infrastructure as Code (IaC) and VM automation with Vagrant.

📬 Contact

If you have any questions or suggestions, feel free to reach out via GitHub.
