Resolution
### Create a customer gateway
1. Create VPC
1. Open the Amazon VPC console.
2. In the navigation pane, under VPN Connections, choose Customer Gateways.
3. Choose Create Customer Gateway.
4. Enter a meaningful name for the customer gateway.
5. Choose an option for Static or Dynamic routing.
6.Enter the public IP address of your customer gateway device.
(Optional) Enter your BGP ASN if you selected the option for dynamic routing.  
8.Choose Yes, Create.


### Create VPC
1. Ensure region is ``Ireland ``

![Step1](images/step%201.png)
### Create a virtual private gateway
1. In the Amazon VPC console, under VPN Connections, choose Virtual Private Gateways.
2. Choose Create Virtual Private Gateway.
3. Enter a meaningful name for the virtual private gateway.
4. Choose Yes, Create.
5. Select the new virtual private gateway and open the context (right-click) menu, and then choose Attach to VPC.


### Create a VPN connection

1. In the Amazon VPC console, under VPN Connections, choose VPN Connections.
2. Select Create VPN Connection.
3. Enter a meaningful name for the VPN connection.
4. For Virtual Private Gateway, choose the virtual private gateway you just created.
5. For Customer Gateway, choose the customer gateway you just created.
6. For Routing Options, choose Dynamic or Static. If you choose static routing, specify the Static IP Prefixes of the appropriate private network(s) on your office LAN.
7.Choose Yes, Create.  
__Get the VPN connection configuration and configure your customer gateway__

## Inside GitBash
1. In the Amazon VPC console, under VPN Connections, choose VPN Connections.
2. Select the VPN connection you created, and then choose Download Configuration.
3. In the Download Configuration dialog box, choose the vendor for the customer gateway, the platform, and the software version, and then choose Yes, Download.
4. Save the text file that contains the VPN configuration. Provide your network administrator with the text file and a link to the related section of the AWS Site-to-Site VPN User Guide. The VPN won't work until the network administrator configures the customer gateway.