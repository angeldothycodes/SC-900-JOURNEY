Let's assume you have setup multiple virtual network that uses a combination of NSGs and Azure Firewall to protect and filter access to assests and resources including Azure Virtual Machines. Now, you are protected from external threats but need to allow your developers and data scientists who are working remotely direct access to those VMs.


In this lesson, we will learn about how Azure Bastion and keyvault can help you achieve that.

In a traditional model, you will need to expose the remote desktop protocol or RDP and SSH to the internet. These protocols can be used to gain remote access to your Virtual machines. This process creates a significant surface threat that can be exploited by the attackers. Azure bastion provides secure and seamless RDP - SSH connectivity to your virtual machine directly from the Azure portal using TLS. When you connect via Azure Bastion, your virtual machines don't need a public IP address, agent, or a special client software


<img width="863" height="394" alt="image" src="https://github.com/user-attachments/assets/936c1a6c-a7db-45bd-a743-55d151800b67" />

## Azure Bastion Features:

> Direct RDP and SSH in Azure portal

> Remote session over TLS and firewall traversal for RDP and SSH

> No public IP required on the Azure VM.

 Azure bastion opens the RDP - SSH connection to your Azure Virtual Machine using private IP on your VM so public IP address is not needed

> No hassle of managing NSGs

A fully managed platform as a service for Azure that harden internally to provide secure RDP - SSH connectivity

> Protection against port scanning

Because you don't need to expose your virtual machine to the internet, VMs are protected against port scanning by rogue and malicious users located outside of your virtual network.

> Protect against zero-day exploits

Because it sits at the perimeter of your virtual network, you don't need to worry about hardening each virtual machine in the virtual network. The Azure platform protects against zero-day exploits by keeping the Azure Bastion hardened and always up to date for you


# Azure Key Vault

Azure Key Vault is a centralized cloud service for storing your application secrets. Key Vault helps to control your application secrets by keeping them in a single central location and providing secure access, commission control, and access logging capabilities.
It's useful for different kind of scenarios:

**1. Secrets management**

You can use your key vault to store securely and tightly control access to tokens, passwords, certificates, API keys, and other secrets.

**2. Key management**

Using Key Vault as a key management solution makes it easier to create and control the encryption keys used to encrypt your data

**3. Certificate management**

Key Vault lets you provision, manage, and deploy your public and private SSL and TLS certificate for Azure and internally connected resources more easily 

**4. Store secrets backed by HW or SW**

The use of Hardware Security Modules (HSMs). The secrets and keys can be protected either by software or by FIBS 140-2 level 2 validated HSMs


=======================
**Azure Key Vault** enforces transport layer security which is known as TLS protocol to protect data when it's travelling between Azure Key Vault and clients. Clients negotiate a TLS connection with Azure Key Vault.

![Uploading image.png…]()

