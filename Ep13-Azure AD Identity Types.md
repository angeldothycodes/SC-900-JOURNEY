**Azure AD** manages different types of users, service principal, manage identities, and devices.


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

