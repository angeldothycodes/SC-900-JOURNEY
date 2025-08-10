Azure Firewall is a managed cloud-based network security service that protects your Azure Virtual network resources. It's a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability.

You can deploy Azure firewall on any virtual network but the best approach is to use it on a centralized virtual network.

All your other virtual and on-premises network will then route through it. The advantage of this model is the ability to centrally exert control of network traffic for all your VNETs across different subscriptions.

With Azure Firewall, you can scale-up the usage to accommodte changing network traffic flows so you don't need to budget for peak traffic.


<img width="860" height="451" alt="image" src="https://github.com/user-attachments/assets/dbea7fe0-bfdc-4085-b313-be9408fba271" />


## Azure Firewall Key Features:

**> Built-in High Availibility & Availability Zones**

High Availablity is built-in so there is nothing to configure. Also, Azure Firewall can be configured to span multiple availability zone for increased availability 


**> Outbound SNAT and Inbound DNAT**

SNAT and DNAT can be used to communicate with internet resources.


**> Threat Intelligence** 

Threat intelligence based filtering can be enabled for your firewall to alert and deny traffic to and from known malicious IP addresses and domains


**> Network & Application-level filtering**

IP addresses, port, and protocol can be used to support fully qualified domain name (FQDN) filtering for outbound traffic and network filtering controls

**> Multiple public IP addresses**

Multiple public IP addresses up to 250 can be associated with your firewall


**> Integration with Azure Monitor**

Integration with Azure monitor enable you to collecting, analyzing, and acting on telemetry from Azure Firewall logs


## Web application Firewall (WAF)

Web application firewall provides centralized protection of your web application from common exploits and vulnerabilities. A centralized WAF helps make security management simpler and improves the response time to your security threat and allows patching a known vulnerability in one place instead of securing a web application.
A web application firewall also gives application administrators better assurance of protection against threats and intrusions. 
WAF can be deployed to Azure application gateway, Azure Front Door, and Azure content Delivery Network. 
You can use Azure Web application Firewall to achieve centralized protection for your web application from common exploits and vulnerabilities.


<img width="864" height="464" alt="image" src="https://github.com/user-attachments/assets/461ac97d-fa90-4fa5-a75f-65fe4634e8cd" />


**Azure Firewall Premium** is a next generation firewall with capabilities that are required for highly sensitive and regulated environments. These capabilities include TLS injection, IDPS, URL Filtering, and Web categories.
