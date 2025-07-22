One way to mitigate against common cybersecurity threat is to encrypt sensitive and valuable data.

**Encryption** is the process of making data unreadable and unusable to unauthorized viewers. To use encrypted data, it must be decrypted which requires the use of security key and the next thing we are going to learn about this lesson is **hashing**

**Hashing** is the process of transforming any given key or a string of numbers into another value. 

The next topic we are going to learn is digital signature or signing. **Digital signature** is a mathematical scheme for demonstrating the authenticity of digital messages or documents


<img width="790" height="246" alt="image" src="https://github.com/user-attachments/assets/9b690215-e702-41b2-a2ce-f5fc9c64d7dd" />


**Asymmetric** encryption is used for things like transport layered security which is known as **TLS** such as https protocol and data signing.

**Encryption** may protect data at rest or in transit.

When it comes to encryption, we need to understand two concepts:
**Encryption ate Rest** and **Encryption in Transit**


**Data at rest** is the data that's stored on a physical device such as a serrver. It may be stored in a database or a storage account but regardless of where it is stored, encryption of data at rest ensures that the data is unreadable without the keys and secrets needed to decrypt it


**Data in transit** is the data moving from one location to another such as across the internet or through a private network. Secure transfer can be handled by several different layers. It can be done by encrypting the data at the application layer before sending it over a network. Https is an example of encryption in transit. Encrypting data in transit protects it from outside and provides a mechanism to transmit data while limiting risk of exposure


# 🔐 What is Hashing?

Hashing is a way to turn data (like a password) into a fixed-length string of characters using a special algorithm. This string is called a hash.
•	If you hash the same input (e.g., "mypassword") using the same algorithm, you’ll always get the same hash.
•	But if you change even one character (e.g., "mypassword1"), the hash will be completely different.
•	Hashing is one-way — you can’t reverse it to get the original data back.
________________________________________

### 🔑 Hashing vs. Encryption

| Feature      | Hashing                              | Encryption                        |
|--------------|--------------------------------------|-----------------------------------|
| Direction    | One-way (can’t be reversed)          | Two-way (can be decrypted)        |
| Uses Keys?   | No                                   | Yes                               |
| Purpose      | Data integrity, password storage     | Data confidentiality              |

________________________________________
🧠 Why Use Hashing for Passwords?
When a user creates a password:
1.	The system hashes it and stores the hash.
2.	Later, when the user logs in, the system hashes the entered password again.
3.	It compares the new hash to the stored one.
4.	If they match, the password is correct — without ever storing the actual password.




<img width="823" height="435" alt="image" src="https://github.com/user-attachments/assets/ff8c79a7-61c0-4637-9eb3-3f51169736f0" />

**Hashing is a process that uses an algorithm to convert original text (like a password) into a unique, fixed-length string called a hash value.**
•	Every time the same text is hashed using the same algorithm, it produces the same hash.
•	This hash acts like a unique fingerprint for the original data.
Hashing is different from encryption:
•	Hashing doesn’t use keys.
•	You can’t reverse a hash to get the original text back.
•	It’s a one-way process.
Why is hashing used for passwords?
When a user creates a password:
1.	The system hashes it and stores the hash.
2.	Later, when the user logs in, the system hashes the entered password again.
3.	It compares the new hash to the stored one.
4.	If they match, the password is correct.






# ✍️ Digital Signing
Digital signing is a way to verify:
•	That a message was sent by the claimed sender.
•	That the message hasn’t been tampered with.
Signing a message:
•	Does not encrypt or change the message itself.
•	Instead, it creates a digital signature — a unique string based on the message and the sender’s private key.
This signature can be:
•	Sent along with the message, or
•	Sent separately.
The receiver uses the sender’s public key to verify the signature. If it checks out, it confirms:
•	The message came from the sender.
•	The content is unchanged.
________________________________________
🛠️ Steps in Creating and Verifying a Digital Signature
1.	Hashing the Message
•	A hash value is generated from the original message using a hashing algorithm.
2.	Signing the Hash
•	The sender uses their private key to sign the hash. This creates the digital signature.
3.	Verifying the Signature
•	The receiver:
•	Hashes the received message again.
•	Uses the sender’s public key to decrypt the digital signature.
•	Compares the decrypted hash with the newly generated hash.
•	If they match, the message is authentic and hasn’t been altered.

