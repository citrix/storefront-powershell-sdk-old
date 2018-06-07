#Disable-STFAuthenticationServiceProtocol
Disable an authentication protocol
##Syntax
```
```
##Detailed Description
Disable one or more authentication protocols on the specified Authentication service.
##Related Commands
*[Enable-STFAuthenticationServiceProtocol](Enable-STFAuthenticationServiceProtocol)
*[Remove-STFAuthenticationServiceProtocol](Remove-STFAuthenticationServiceProtocol)
*[Get-STFAuthenticationProtocolsAvailable](Get-STFAuthenticationProtocolsAvailable)
*[Add-STFAuthenticationServiceProtocol](Add-STFAuthenticationServiceProtocol)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String[]
Parameter Name: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
##Return Values
##Examples
###EXAMPLE 1 Disable all authentication protocols
```
```
REMARKS
Disable all authentication protocols for the only configured Authentication service.

```
```
REMARKS
Disable the HttpBasic authentication protocol.
