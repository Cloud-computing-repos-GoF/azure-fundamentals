### Networking Fundamentals

- Azure Virtual Networks:     
    Benefits:   
    1. Isolation and Segmentation (subnets)     
    2. Internet Communications   
    3. Communicate between Azure Resources (Virtual Networks, service Endpoints)     
    4. Communicate with on-premises resources (point2site vpn, site2site vpn, ExpressRoute)  
    5. Route Network Traffic   
    6. Filter Network Traffic (Network Security Groups, Network Virtual Appliances)    
    7. Connect Virtual Networks   

- Azure VPN Gateway :
    1. policy-based    
    2. Route-based :   
        * IKEv2 support   
        * Wildcard traffic selector   
        * Dynamic routing protocols 

    - Sizes:

    |**SKU (Stop Keeping Unit)**|**Site2site Network2network tunnels**| **Aggregate throughput benchmark**| **Border Gateway protocol**|
    |:---:|:---:|:---:|:---:|
    |Basic| Max 10| 100 Mbps| Not Supported|
    |VpnGW1|30|650Mbps|Supported|
    |VpnGW2|30|1Gbps|Supported|
    |VpnGW3|30|1.25 Gbps| Supported|


    - Requirements:
         1. Virtual Network Vnet
         2. Gateway subnet   
         3. Public IP address   
         4. Local Network Gateway  
         5. Virtual Network Gateway   
         6. Connection Resource    


![Responsibility Levels for Services](https://github.com/Cloud-computing-repos-GoF/azure-fundamentals/blob/master/images/vpn_azure.png)

- Azure ExpressRoute


DNS Communications   
UDR  
network Security Group  
Route Table  


[Additional readings](https://www.coursera.org/learn/microsoft-azure-cloud-services/supplement/raOsc/additional-reading)
