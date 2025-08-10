Azure supports various encryption models including server-side encryption that uses service managed keys, customer managed keys in key vault, or customer managed keys on customer-controlled hardware which is client-side encryption.

With client-side encryption, you can manage and store keys on on-premises or other secure location.

# Encryption on Azure

Microsoft Azure provides many different ways to secure your data each depending on the service or usage required.

## Azure Storage Service Encryption

Data-at-rest in Azure blob storage and Azure File shares can be encrypted in both server-side and client-side scenarios. Azure storage service encryption or SSE can automatically encrypt data before it is stored.
It automatically decrypts the data when you retrieve it. The process is completely transparent to users. 
**Storage Service Encryption** uses 256 AES encryption which is one of the strongest block ciphers available in the world. AES handles encryption, decryption, and key management transparently. 


## Azure Disk Encryption

You can protect windoes and Linux virtual machine by using Azure Disk Encryption which uses Windows bitlocker technology and Linux uses dm-crypt to protect both operating system disk and data disk with full volume encryption.
Encryption keys secrets are safeguarded in your Azure key vault subscription.
By using Azure Backup Service, you can backup and restore encrypted virtual machines that uses key encryption key configuration. It is known as AEK configuration as well.

## Transparent Data Encryption (TDE)

TDE is used to encrypt SQL server, Azure SQL database and Azure synapse analytics data files in real-time. Using a database encryption key or DEK which is stored i the database boot record for availability during recovery. TDE protects data and log files using AES and 3DES encryption algorithm.

Encryption of database file is performed at the page-level. The pages in an encrypted database are encrypted before they are written to the disk and decrypted when they are read into memory. TDE is now enabled by default on newly created Azure SQL databases.

Espionage, data theft, and data exfiltration are real threat to any company. The loss of sensitive data can be crippling and have legal implications. 
For most organizations data is their most valuable asset. In a leyered security strategy, the use of encryption serves as the last and the strongest line of defense.


