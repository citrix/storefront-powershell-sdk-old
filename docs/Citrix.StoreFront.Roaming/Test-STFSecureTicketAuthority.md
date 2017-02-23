#Test-STFSecureTicketAuthority
Validate a NetScaler gateway STA configuration
##Syntax
```
```
##Detailed Description
Validate a PowerShell object populated with a NetScaler gateway STA configuration.
##Related Commands
*[Read-STFNetScalerConfiguration](Read-STFNetScalerConfiguration)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.IStaServerData
Parameter StaConfigurationObject: The .NET 'Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.IStaServerData' reference type
##Return Values
###StaValidationStatus
The .NET 'Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.StaValidationStatus' reference type
##Notes
Any specified STA servers will be contacted during validation. A Secure Ticket Authority id is used to uniquely identify an STA server used for remote access.
##Examples
###EXAMPLE 1 Validate a NetScaler gateway STA configuration
```
$stasToUpdate = Test-STFSecureTicketAuthority -StaConfigurationObject $netscalerConfiguration
```
REMARKS
Returns a list of STA servers with a validation status indicating success or failure including incorrect STA
authorities.
The STA url provided by NetScaler may not resolve on an internal network so will need updating to a StoreFront local
address.
The STA authority must match that provided in the NetScaler configuration export.

```
$stasToUpdate = Test-STFSecureTicketAuthority -StaConfigurationObject $netscalerConfiguration
```
REMARKS
Returns a list of STA servers with a validation status indicating success or failure including incorrect STA
authorities.
The STA url provided by NetScaler may not resolve on an internal network so will need updating to a StoreFront local
address.
The STA authority must match that provided in the NetScaler configuration export. The expected output in the example
shows both a valid and invalid STA url location.
OUTPUT
```
'STA0000'.


StaUrl                      : http://www.example.com/scripts/ctxsta.dll
ConfigurationStaAuthorityId : STA0000
DetectedStaAuthorityId      : STACB1DA97D3546
ResultCode                  : AuthorityId Mismatch
IsValid                     : False

StaUrl                      : http://xendesktop.company.com/scripts/ctxsta.dll
ConfigurationStaAuthorityId :
DetectedStaAuthorityId      : STA578994219
ResultCode                  : Success
IsValid                     : True
```