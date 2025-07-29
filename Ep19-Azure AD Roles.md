**Global administrator**, users with this role have access to all administrative features in Azure AD.
The person who signs up for the Azure AD tenant automatically becomes a global administrator.


**User Administrator**. User with this role can create and manage all aspects of users and groups. Additionally, this role include the ability to manage support tickets and monitor service health.


**Billing Administrator**. Users with this role makes purchases manage a subscription and manages support tickets an monitors service health.


## Azure AD Built-in Roles
There are many different built-in roles for different areas of responsibility. All built-in roles are pre-configured bundles of permissions designed for specific tasks.


## Azure AD Custom Roles
Custom Roles give flexibility when granting access. Granting permission using custom Azure AD roles is a two-step process that involves creating a custom role definition which consists of a collection of permissions that you add from a preset list.


Once you have created a role definition, you can assign it to a user by creating a role assignment.
A **role assignment** grants the user the permission in a role definition at a specific scope. A custom role can be assigned at org wide scope meaning that the role member has the role permission over all resources in the organziation. 
A custom role can also be assigned at an object scope. An example of an object scope would be a single application.

**Azure custom roles require an Azure AD P1 or P2 license.**

## Azure AD RBAC

When you create these custom roles or when you decide to assign a rights to a user, only grant the access the user needs. It's a best practice and more secure to grant users least privilege to get their work done. This means that if somebody mostly manages users, you should assign the user administrator role and nor global administrator. 
This mitigates the risk of a user account being compromised and a hacker locking you out of your account.
By assigning least privileges, you limit the damage that could be done with a compromised account.

Managing access using role is known as Role Based Access Control (**RBAC**). Azure AD built-in roles are a form or RBAC to control Azure AD resources. 
