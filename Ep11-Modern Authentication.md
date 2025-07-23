**Modern authentication** is the umbrella term for authentication and authorization.
Between a client such as your laptop or a phone and a server such as a website or an application. At the center of the modern authentication is the **role of an identity provider**


<img width="835" height="473" alt="image" src="https://github.com/user-attachments/assets/07d291b5-b71d-478d-8a43-6e1243e928a9" />


With modern authentication, all services, including all authentication services are provided by a central identity provider. An identity provider creates, maintains, and manages identity information while providing authentication, authorization, and auditing services. The information that is used to authenticate the user with the server is stored and managed centrally by the identity provider. With the central identity provider, organization can establish authentication and authorization policies, monitor user behavior, identify suspicious activities and reduce malicious attacks. Microsoft Azure Active Directory is an example of a cloud-based identity provider. Other examples of identiy provider are Twitter, Google, Amazon, LinkedIn, GitHub, etc.


<img width="865" height="482" alt="image" src="https://github.com/user-attachments/assets/c72088aa-8085-42eb-9222-77abe1e8ab8f" />






## The Concept of Federated Services

<img width="880" height="459" alt="image" src="https://github.com/user-attachments/assets/a0cfd4b0-04c7-426a-a626-20d89bff88d0" />

What is Single Sign-On (SSO)? Another capability of identity provider and moden authentication is the support of Single Sign-On or known as SSO. With Single Sign-On, the user logs in once and their credentials is used to access multiple applications and resources. 

**When you set up Single Sign-On to work between multiple identiy providers, it is called Federation**

**Federation** enables the access of services across organizational or domain boundaries by establishing trust relationship between the respective domains identity provider.
With federation, there is no need for a user to maintain a different username and password when accessing resources in other domains. 

The simplified way to think about the federation scenario is 
- the website uses the authentication services of an identity provider.
- The user authenticates with the Identity provider
- The identity provider has a trust relationship configured with the user authentication
- And when the user credentials are passed to the website, the website trusts the user and allows them access


With federation, trust is not always bi-directional. A common example of a federation in practice is when a user login to a third-party site with their social media account such as Twitter.
In this scenario, twitter is an identity provider and the third-party website may be using different identity provider such as Azure Active Directory. So there is a trust relationship between Azure AD and Twitter



## The Concept of Directory Services and Active Directory

In the context of computer network, a directory is a hierarchical structure that stores information about the object in the network. A **Directory service** stores directory data and makes this data available to network users, administrators, services, and applications.

Active Directory is a set of directory services developed by Microsoft as part of Windows 2000 for on-premises domain based networks.
The best known active directory service is Active Directory Domain Service or ADDS. It stores about members of domain including devices and users and verifies their credentials and defines their access rights.

A server running ADDS is a domai controller or known as Domain Server.

**ADDS** is a central componnet in organization with on-premises IT infrastructure. ADDS gives organization the ability to manage multiple on-premises infrastructure components and systems using a single identity per user. 
ADDS does not however support mobile devices, SaaS applications, or line of business applications that require modern authentication medthods


**What is the reason for modern authentication?** Because there was a growth of cloud services, SaaS application, and personal devices being used at work has resulted in the need for modern authentication and an evolution of Active Directory based identity solutions.

**Azure Active Directory** is the next evolution of identity and access mnagement solutions by providing organizations with an identity as a service solution for all their apps across cloud and on-premises
