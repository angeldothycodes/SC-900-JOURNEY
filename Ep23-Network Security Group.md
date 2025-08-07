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
