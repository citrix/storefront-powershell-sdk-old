#Get-STFWebReceiverClientPlugin
Gets the plug-in definitions configured within the WebReceiver service
##Syntax
```
```
##Detailed Description
Gets the Client plug-in definitions configured within the WebReceiver service
##Related Commands
*[New-STFWebReceiverClientPlugin](New-STFWebReceiverClientPlugin)
*[Add-STFWebReceiverClientPlugin](Add-STFWebReceiverClientPlugin)
*[Clear-STFWebReceiverClientPlugin](Clear-STFWebReceiverClientPlugin)
*[Remove-STFWebReceiverClientPlugin](Remove-STFWebReceiverClientPlugin)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###ClientPlugin
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.ClientPlugin' reference type
##Examples
###EXAMPLE 1 Get the WebReceiver plugins
```
Get-STFWebReceiverClientPlugin -WebReceiverService $webReceiver
```
REMARKS
Get the client plug-ins configured for the only WebReceiver service.
OUTPUT
```
Source     : /plugins/netscalar/script1.js
Scripts    : {Citrix.StoreFront.Model.ReceiverForWeb.ClientScript, Citrix.StoreFront.Model.ReceiverForWeb.ClientScript}
Styles     : {Citrix.StoreFront.Model.ReceiverForWeb.ClientStyle, Citrix.StoreFront.Model.ReceiverForWeb.ClientStyle}
Parameters : {param1, param2}
```