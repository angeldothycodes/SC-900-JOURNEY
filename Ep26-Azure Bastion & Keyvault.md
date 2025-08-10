Let's assume you have setup multiple virtual network that uses a combination of NSGs and Azure Firewall to protect and filter access to assests and resources including Azure Virtual Machines. Now, you are protected from external threats but need to allow your developers and data scientists who are working remotely direct access to those VMs.


In this lesson, we will learn about how Azure Bastion and keyvault can help you achieve that.

In a traditional model, you will need to expose the remote desktop protocol or RDP and SSH to the internet. These protocols can be used to gain remote access to your Virtual machines. This process creates a significant surface threat that can be exploited by the attackers. Azure bastion provides secure and seamless RDP - SSH connectivity to your virtual amchine directly from the Azure portal
