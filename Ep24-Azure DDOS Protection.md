The aim of Distributed Denial of Service or DDos Attack is to overwhelm the resource on your application and server making them unresponsive or slow for genuine users.

A DDoS attack will usually target any public facing endpoint that can be accessed through the internet. There are three most popular type of Distributed Denial of Service attack. 

**1. Volumetric attacks**

**2. Protocol attacks**

**3. Resource (application) layer attacks**


## Volumetric Attacks
These are volume-based attacks that flood the network with seemingly legitimate traffic. Overwhelming the available bandwidth, legitimate traffic isn't able to get through. These types of attacks are emasured in bits-per-seconds.



## Protocol Attacks
Protocol attacks render a target inaccessible by exhausting server resources with false protocol requests that exploit weakness in layer 3 network and layer 4 protocols. These types of attacks are typically measured in packets per second.



## Resource or Application Layer Attacks

 These attacks target web application packets to disrupt the transmission of data between the host


 <img width="863" height="475" alt="image" src="https://github.com/user-attachments/assets/7d2b0a8a-7607-44c3-b712-aaf14fb70bdf" />

 
# Azure DDoS Protection

**Azure DDoS Protection service** is designed to help protect your application and servers by analyzing network traffic and discarding anything that looks like a DDoS attack.

**Azure DDoS Protection** identifies the attacker's attempt to overwhelm the network. It blocks the traffic from the attacker and ensuring the traffic never reaches the Azure resources. Legitimate traffic still flows to Azure without any ibterruption of service. 
Azure DDoS protection uses the scale and elasticity of Microosft Global Network to bring DDoS mitigation capability to every Azure region.  During a DDoS attack, Azure can scale your computing needs to meet the demand.
DDoS protection can manage your cloud consumption by ensuring that your network load only reflects actual customer usage.


Azure DDoS comes in two tiers, **Basic** and **Standard**:

<img width="591" height="250" alt="image" src="https://github.com/user-attachments/assets/fe458e28-3207-4845-9f3b-1f56b7b80891" />

The basic tier is automatically enabled for every property in Azure at no additional cost. 
Always-on traffic monitoring and real-time mitigation of common network level attacks provide the same defenses that Microsoft online services use.

The standard tier provides extra mitigation capabilities that are tied specifically for Microsoft Azure virtual network resources. DDoS protection standard is simple to enable and requires no application changes. The protection policies are tuned through dedicated traffic monitoring and machine learning algorithms. Policies are applied to public IP addresses which are associated with resources deployed in virtual networks such as Azure Load Balancer and Application Gateway.


Use Azure DDoS to enable you to protect your devices and application by analyzing traffic across your network and taking appropriate action on suspicious traffic.

**DDoS protection** is enabled at virtual network level. All protected resource types within Azure Virtual Network will be automatically protected when DDoS protection is enabled on the Azure Virtual Network. 

When application gateway with WAF is deployed in your DDoS protected VNet, there are no additional charges for WAF. You pay for application gateway at the lowest non-VAT rate
