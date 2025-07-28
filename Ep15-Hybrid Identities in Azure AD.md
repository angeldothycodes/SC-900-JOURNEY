Organizations may use hybrid identity model or cloud only identity model. 

In the hybrid model, identities are created in Windows Active Directory and then synchronized to Azure Active Directory.

In the cloud-only model, identities are created wholly and managed in Azure Active Directory. 

So whether identities are created on-premises or in the cloud, users can access both cloud and on-premises resources. 

In this lesson, we are going to learn about concepts of hybrid identities and three authentication methods. 


<img width="823" height="422" alt="image" src="https://github.com/user-attachments/assets/f96bb55e-7079-45ca-bdc6-9def60bdb7ba" />


With the hybrid model, users accessing both on-premises and cloud apps are hybrid users managed in the on-premises Active Directory. When you make an update in your on-premises ADDS, all updates to user accounts, groups, and contacts are synchronized to your Active Directory.

Synchronization is managed with your Azure Active Directory. The synchronization is managed with your Azure ACtive Directory connect, when using the hybrid model, the authenticationc can either be done by Azure Active Directory which is known as managed authentication or Azure AD redirects the client request authentication to another directory provider which is known as federated authentication.



There are three types of authentication methods used here:

>> Password hash synchronization
>> Pass-through authentication (PTA)
>> Federation authentication


**Password hash Synchronization**. This is the simplest way to enable authentication for on-premises directory objects in Azure Active Directory. Users can use the same username and password that they use on-premises without any additional infrastructure be needed.
Password Hash Syncrhonization is a type of managed authentication.

**Pass-Through Authentication** provides a simple password validation for Azure Active Directory Authentication Service by using a software agent that runs on one or more on-premises servers. The servers validate the users directy with on-premises Active Directory which ensures that the password validation doesn't happen in the cloud. 
The pass-through authentication is a type of managed authentication.

**Federated Authentication**. Azure Active Directory hand off this authentication process to a separate trusted authentication system such as an on-premises Active Directory Federation Services (**ADFS**). **ADFS** is used to validate the user's password in this scenario.

To meet various business security and technical requirements, organization can choose between password hash synchornization, pass-through authentication, and federation authentication. You should always consider each of this authentication in the design process before you choose one.

