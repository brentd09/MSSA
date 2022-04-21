
# Lab 12: Service Endpoints and Securing Storage


## Task 3



8. On the **Add outbound security rule** blade, specify the following settings to explicitly allow outbound traffic to Azure Storage (leave all other values with their default settings): 

    |Setting|Value|
    |---|---|
    |Source|**Service Tag**|
    |Source service tag|**VirtualNetwork**|
    |Source port ranges|**\***|
    |Destination|**Service Tag**|
    |Destination service tag|**Storage**|
    |Destination port ranges|**\***|
    |Protocol|**Any**|
    |Action|**Allow**|
    |Priority|**1000**|
    |Name|**Allow-Storage-All**|

9. On the **Add outbound security rule** blade, click **Add** to create the new outbound rule. 

10.

11. On the **Add outbound security rule** blade, specify the following settings to explicitly deny outbound traffic to Internet (leave all other values with their default settings): 

    |Setting|Value|
    |---|---|
    |Source|**Service Tag**|
    |Source service tag|**VirtualNetwork**|
    |Source port ranges|**\***|
    |Destination|**Service Tag**|
    |Destination service tag|**Internet**|
    |Destination port ranges|**\***|
    |Protocol|**Any**|
    |Action|**Deny**|
    |Priority|**1100**|
    |Name|**Deny-Internet-All**|
    
12. fklkdfkl

13. On the **Add inbound security rule** blade, specify the following settings (leave all other values with their default values): 

    |Setting|Value|
    |---|---|
    |Source|**Any**|
    |Source port ranges|**\***|
    |Destination|**Service Tag**|
    |Destination service tag|**VirtualNetwork**|
    |Destination port ranges|**3389**|
    |Protocol|**TCP**|
    |Action|**Allow**|
    |Priority|**1200**|                                                    
    |Name|**Allow-RDP-All**|



