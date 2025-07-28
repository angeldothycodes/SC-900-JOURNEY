**Authentication** is the process of verifying an identity to be legitimate. Legacy applications have relied on a single form of authentication and most often, a password. However, passwords are problematic for users and easy to be compromsied.
**Multi-factor AUthentication (MFA)** requires more than one form of verification to prove that an identity is legitimate so that means that even when an identity password has been compromised, a hacker cannot gain entry to a resource.

<img width="902" height="486" alt="image" src="https://github.com/user-attachments/assets/426290ae-af27-4c67-a0f2-7be306ca8881" />

 
An MFA prompts are configrued to be part of your Azure Active Directory sign-in event. Azure Active Directory automatically requests and processes multi-factor authentication without you making any changes to your applications or services. When a user signs in, they receive a multi-factor authentication prompt and choose from one of the additional verification forms that they have registered.


### MFA IN AZURE AD

<img width="875" height="376" alt="image" src="https://github.com/user-attachments/assets/5b981ecb-eef5-4757-8c8a-d81ba7522281" />


### Passwordless Authentication (Something You Are)

<img width="835" height="462" alt="image" src="https://github.com/user-attachments/assets/54e0cd14-ebe0-4568-98dc-8a1c2b1ac314" />


<img width="874" height="466" alt="image" src="https://github.com/user-attachments/assets/0a779094-5ccc-4a63-990a-7a8cb317d246" />


### Windows Hello

Windows Hello lets users authenticate to a Microsoft account, an Active Directory account, and Azure Active Directory account, and Identity Provider services or relying party services that support fast ID online or FIDO version 2.0.


**Why is Windows Hello safer than a password?**
The Windows Hello pin is backed by a trusted platform module or known as TPM chip which is a secure crypto processor that is designed to carry out cryptographic operations. The chip includes multiple physical security mechanisms to make it tamper resistant and malicious software is unable to tamper with the security functions of the TPM. Many mobile phones and laptops have TPM chip.



### Self-Service Password Reset

Self-service password reset is a feature of Azure Active Directory that allows users to change or reset their password without administrator or help desk involvement.
If a user is locked or they have forogotten their password, users can follow a prompt to reset their password and get back to work.


<img width="554" height="437" alt="image" src="https://github.com/user-attachments/assets/d2df9a80-8f08-474f-8807-04cf34b9acae" />






