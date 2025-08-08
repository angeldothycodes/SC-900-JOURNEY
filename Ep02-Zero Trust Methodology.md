# ✍️ Zero trust Methodolgy

<img width="868" height="493" alt="image" src="https://github.com/user-attachments/assets/db9cd51f-39fe-41be-a07f-d9b3ab9e5d0b" />


- **Zero Trust** assumes everything is an open and untrusted network, even resources behind the firewalls of the corporate network.

- **Zero Trust model** operates on the principle of **trust no one, verify everything**.

- The attacker's ability to bypass conventional access control is ending by illusion that traditional security strategies are sufficient. By no longer trusting the integrity of the corporate network, security is strengtened.
- 
- In practice, this means that we no longer assume that a password is sufficient to validate a user so we add a **multi-factor authentication** to provide additional checks.

- Instead of granting access to all devices on the corporate network, users are allowed only to specific application or data that they need.


  ## 🐣 Zero Trust Guiding Principles

  <img width="515" height="442" alt="image" src="https://github.com/user-attachments/assets/1910f53e-ef5a-4598-a40b-b88bc0d193bb" />


  The **Zero Trust model** has three principles which guide and underpin how security is implemented. These are:

  - **Verify explicitly**
  - Using **Least Privileged access** all the time
  - **Assume Breach**
 
What does it mean to **verify explicitly**? You should always authenticate and authorize based on the available data points including user identity, location, device, security or workload, data classification and any other anomalies.

The second principle is **least privileged access**. This means that you should limit user access with just enough time and acess which is known as **JET** or **JEA**. Other ways you can limit the privileged access is by implementing risk-based adapative policies and data protection to protect both data and productivity.

The final guiding principle is **assume breach** all the time. You should segment access by network, user, devices, and application. We should use encryption to protect data and use analytics to gain visbility and detect threats and improve your security posture.


In the zero trust model, all elements work together to provide end-to-end security. These **six elements** are the foundational pillars of the zero trust model which includes **identities, devices/ endpoints, data, apps, infrastructure, and network**.

<img width="806" height="489" alt="image" src="https://github.com/user-attachments/assets/7918b3f6-5aa9-48a7-b9be-7153b2cec75a" />


**Let's look into IDENTITIES.**

<img width="802" height="445" alt="image" src="https://github.com/user-attachments/assets/f07b61ca-eb1a-485f-8ea2-cf229fcf38f8" />

These identities may be users, services, or devices. When an identity attempts to access a resource, it must be verified with strong authentication and follow least privileged access principles.


**DEVICES/ENDPOINTS**

These devices and workloads create a large attack surface as data flows from devices to on-premises workloads and the cloud. Monitoring devices for health and compliance is important aspect of security.


**DATA**
Data should be classified, labeled, and encrypted based on its attributes. Security efforts are ultimately about protecting data and ensuring it remains safe when it leaves devices, applications, infrastructure, and networks that the organization controls.


**APPLICATION**
Application are the way that data is consumed. This includes discovering all applications being used sometimes called **shadow IT** because not all applications are managed centrally. This pillar also includes managing permissions and access.


**INFRASTRUCTURE**

To improve security, you access for version configurationa nd just in time access and use telemetry to detect attacks and anomalies. This allows you to automatically block or flag risky behavior and take proactive actions.



**NETWORK**

The sixth foundational pillar for the zero trust model is **network**. **Networks** should be segmented including deeper in-network micro segmentation, also real-time protection, end-to-end encryption, monitoring, and analytics should be employed as well.



**THESE SIX FOUNDATIONAL PILLARS WORK TOGETHER WITH THE ZERO TRUST MODEL TO ENFORCE ORGANIZATIONAL SECURITY POLICIES**

Organizations that operate with zero trust mentality are more resilient, consistent, and responsive to new attacks. A true end-to-end zero trust strategy not only makes it harder for attackers to get into the network bu also minimizes potential blast radius by preventing any lateral movement. That's why zero trust methodology is very important and you should always think about when you design solution in the cloud.
