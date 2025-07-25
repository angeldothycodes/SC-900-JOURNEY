**Azure AD** manages different types of users, service principal, managed identities, and devices.


<img width="887" height="461" alt="image" src="https://github.com/user-attachments/assets/b5f6d219-d6db-4d13-867c-541972ac9038" />


## User

**Azure Active Directory users**. A user identity is a representation of something that is managed by Azure Active Directory. Employers and guests are represented as users in Azure Active Directory. If you have several users with the same access needs, you can create group in Azure Active Directory.

**Groups** allow you to assign access permission to all the members of the group instead of having to assign the access rights individually. 

**Azure AD business to business which is known as B2B collaboration** is a feature within external identities which include the capability to add guests user into your Azure Active Direcoty. With B2B collaboration, an organization can securely share applications and service users from other organizations.


## Service Principal

A **security principal** is a securiy identity used by applications or services to access specific Azure resources. You can think of it as an identity for an application.
For an application to delegate its identity and access functions to Azure AD, the application must first be registered with the Azure Active Directory. The process of registering the application creates a globally unique object ID which is stored in your home tenant or directory. A service principal is created in each tenant where the application is used and references the global unqiue object ID.
The service principal defines what the app can do in the tenant such as who can access the app and what resources the app can access


## Managed Identity

A managed identity is an identity in Azure Active Directory that is automatically managed by Azure. Managed identities are typically used to manage the credentials for authenticating a cloud applicaion with an Azure service. 
**What are the benefits to using managed identity?** 
- Application developers can authenticate to services that support managed identity or Azure resources

- Any Azure service that supports Azure AD authentication can use managed identities to authenticate to another Azure service. For example, accessing your Azure key vault

- Managed identities can be used without any additional cost as well.


##### There are two types of managed identites:
> **System assigned**. Some Azure services allows you to enable a managed identity directly on a service instance. When you enable a system assigned managed identity, an identity is created in Azure Active Directory that is tied to the lifecycle of the service instance. When the resource is deleted, Azure automatically deletes the identity for you. By design, only that Azure resource can use this identity to request token from Azure AD

> **User assigned**. You may also create a managed identity as a standalone Azure resource. A user assigned managed identity is assigned to one or more instances of an Azure service. You can create user as signed managed identity and assign it to one or more instances of an Azure service. In the case of user assigned managed identities, the identity is managed separately from the resources that uses it.



## Device

A device is a piece of hardware such as a mobile device, laptop, server, or printer. Device identities can be set up in different ways in Azure Active Directory which determine the properties such as who owns the device. Managing devcies in Azure AD allows an organization to protect its assets by using tools such as Microsoft Intune to ensure standards of security and compliance. Azure AD also enables single sign-on to these devices (SSO), apps, and services anywhere through these devices. 

When you talk about these devices, there are multiple options for getting these devices into Azure AD:

1. **Azure AD Registered devices**. These can be Windows 10, IoS, Android, or Mac operating system devices. Devices that are Azure AD registered are typically owned personally rather than by the organization. They are signed in with a personal Microsoft account or another local type.

2. **Azure AD joined**. These devices exist only in the cloud. Azure AD joined devices are owned by an organization's Azure AD account. Users sign in to their devices with their Azure AD or synced Azure Active Directory work or school accounts. You can configure Azure AD joined devices for all Windows 10 devices except for Windows 10 home edition.

3. **Hybrid Azure AD Joined** devices. These can be your Windows 7, 8.1, Windows 10, Windows 11, Windows Server 2008, or newer version of server editions. Devices that are Hybrid Azure AD joined are owned by your organization and signed in with an Azure ACtive Directory domain service belonging to that organization. They exist in the cloud and on-premises. IT Admins can use tools like Microsoft Intune which is a mobile device management solution to manage these devices


# GUIDE/ LAB
<img width="892" height="406" alt="image" src="https://github.com/user-attachments/assets/fe0e90ab-1957-4f6e-a138-9359252de871" />
