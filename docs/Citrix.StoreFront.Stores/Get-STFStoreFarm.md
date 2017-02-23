#Get-STFStoreFarm
Get farm configured for a Store
##Syntax
```
```
##Detailed Description
Get the XenApp\XenDesktop farms configured in the Store service.
##Related Commands
*[Remove-STFStoreFarm](Remove-STFStoreFarm)
*[Add-STFStoreFarm](Add-STFStoreFarm)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.String
Parameter FarmName: The .NET 'System.String' reference type
##Return Values
###Farm
A .NET class representing the configuration of a Farm in StoreFront Store service
##Examples
###EXAMPLE 1 Get all Store farms
```
Get-STFStoreFarm -StoreService $storeservice
```
REMARKS
Get all farms configured in a Store
OUTPUT
```
Port                    : 80
SSLRelayPort            : 443
TransportType           : HTTP
LoadBalance             : True
FarmType                : XenApp
Servers                 : {xa65}
AllFailedBypassDuration : 0
BypassDuration          : 60
TicketTimeToLive        : 100
RadeTicketTimeToLive    : 100

FarmName                : Controller2
Port                    : 80
SSLRelayPort            : 443
TransportType           : HTTP
LoadBalance             : False
FarmType                : XenDesktop
Servers                 : {XD75}
AllFailedBypassDuration : 0
BypassDuration          : 60
TicketTimeToLive        : 100
RadeTicketTimeToLive    : 100
```