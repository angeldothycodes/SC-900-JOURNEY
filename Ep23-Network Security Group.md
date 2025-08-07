Modern work environment where more users work remotely from home, managing access to assets and resources on your Azure virtual network is essential.


**In this lesson, it will be discussed how Azure Network Security Groups can automatically allow or deny traffic to your cloud-based resources and seets**



<img width="835" height="440" alt="image" src="https://github.com/user-attachments/assets/8a756ba5-bbd0-4ba3-950f-69731cb58a1c" />




**Network Security Groups or NSG** let you allow or eny network traffic to and from Azure resources that exist in your Azure Virtual Network, for example a virtual machine. When you create an NSG, it can be associated with multiple subnets or network interfaces in your VNet.

An NSG consists of rules that define how the traffic is filtered. NSG security rules are evaluated by priority using five information points:

> Source
>
> Source Port
>
> Destination
>
> Destination port
>
> Protocol

... to either allow or deny the traffic.

As a guideline, you shouldn't create two security rules with the same priority and direction.

<img width="860" height="468" alt="image" src="https://github.com/user-attachments/assets/f8981e19-abea-42cc-a1f2-7c7c391061ca" />

** every NSG rules need to gave a unique name that describes its purpose. For example, admin access-only filter
** Prioirty column is a number between 100 and 4096. Rules are processed in priority order. With lower number processed before the higher numbers when traffic matches a rule, processing stops. This means that any other rules with a lower priority won't be processed.

<img width="809" height="401" alt="image" src="https://github.com/user-attachments/assets/e190e849-f882-4585-8146-be180181fa76" />


The next one we need to learn about is source or destination. This specifies either individual IP address or IP address range or service tag or application security group. Specifiying a range, a service tag, or applicationv security groups enable you to create a fewer security rules.

Protocol - this indicate what network protocol will the rule check. The protocol can be of any TCP, UDP, ICMP, or any. 

The next thing is direction, whether it is inbound or outbound traffic. Finally, we need to learn about action. Action decide what will happen when this rule is triggered. 


<img width="903" height="459" alt="image" src="https://github.com/user-attachments/assets/838804df-7767-4e99-9f3a-30eca28786d8" />

**There are limits to the number of security rules you can create in an NSG. Use Azure NSGs to automatically allow or deny traffic to yur cloud-based resources and assets.**


**An Azure virtual network is similar to network you would find in your organization. It enables different Azure resources. For instance, an Azure virtual machine to securely communciate with other Vnets. The internet or your on-premises network. A VNet can be divided into multiple subnetworks or it is known as subnets and each with specific resources assigned to them. You can secure the resources within a subnet using network security groups.

