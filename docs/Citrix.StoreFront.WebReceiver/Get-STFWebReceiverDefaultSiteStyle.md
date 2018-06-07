#Get-STFWebReceiverDefaultSiteStyle
Gets the default site styles for the site defined in the default style sheet
##Syntax
```
```
##Detailed Description
The default style information is retrieved from css file of Receiver for Web site. This style is limited to the non-classic experience.
##Related Commands
*[Clear-STFWebReceiverSiteStyle](Clear-STFWebReceiverSiteStyle)
*[Get-STFWebReceiverSiteStyle](Get-STFWebReceiverSiteStyle)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###SiteStyle
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.SiteStyle' reference type
##Examples
###EXAMPLE 1 Get the default site style
```
Get-STFWebReceiverDefaultSiteStyle
```
REMARKS
Get the default site style for the specified WebReceiver service.
OUTPUT
```
C:\inetpub\wwwroot\Citrix\StoreWeb\receiver\images\2x\CitrixReceiverLogo_Home@2x_3FEDFD700D66DF42.png
LogonLogoPath         : 
C:\inetpub\wwwroot\Citrix\StoreWeb\receiver\images\2x\CitrixStoreFront_auth@2x_1B99A8ADCDDFD9AB.png
HeaderBackgroundColor : #574f5b
HeaderForegroundColor : #fff
LinkColor             : #02a1c1
```