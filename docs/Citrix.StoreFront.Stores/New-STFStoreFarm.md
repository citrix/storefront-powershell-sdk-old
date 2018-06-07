#New-STFStoreFarm
Create a new Farm
##Syntax
```
```
##Detailed Description
Create a XenApp \ XenDesktop farm to be added to a Store service.
##Related Commands
*[Remove-STFStoreFarm](Remove-STFStoreFarm)
*[Get-STFStoreFarm](Get-STFStoreFarm)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter FarmName: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.FarmType
Parameter FarmType: The .NET 'Citrix.StoreFront.Model.Store.FarmType' value type
###System.String[]
Parameter Servers: The .NET 'System.String' reference type
###System.String[]
Parameter ServiceUrls: The .NET 'System.String' reference type
###System.Int32
Parameter Port: The .NET 'System.Int32' value type
###Citrix.StoreFront.Model.Store.TransportType
Parameter TransportType: The .NET 'Citrix.StoreFront.Model.Store.TransportType' value type
###System.Int32
Parameter SSLRelayPort: The .NET 'System.Int32' value type
###System.Boolean
Parameter LoadBalance: The .NET 'System.Boolean' value type
###System.Int32
Parameter AllFailedBypassDuration: The .NET 'System.Int32' value type
###System.Int32
Parameter BypassDuration: The .NET 'System.Int32' value type
###System.Int32
Parameter TicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter RadeTicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter MaximumFailedServersPerRequest: The .NET 'System.Int32' value type
###System.String[]
Parameter Zones: The .NET 'System.String' reference type
###System.String
Parameter Product: The .NET 'System.String' reference type
###System.String
Parameter RestrictPoPs: The .NET 'System.String' reference type
###System.String
Parameter FarmGuid: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
###Farm
A .NET class representing the configuration of a Farm in StoreFront Store service
##Examples
###EXAMPLE 1 Create a farm to be added to a Store service
```
```
REMARKS
Adds the Xen1 XenDesktop server to the XenDesktop75 farm
