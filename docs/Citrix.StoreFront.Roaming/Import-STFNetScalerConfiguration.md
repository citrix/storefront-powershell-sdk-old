#Import-STFNetScalerConfiguration
Import a NetScaler remote access configuration
##Syntax
```
```
##Detailed Description
Import a NetScaler remote access configuration supplied by a NetScaler administrator.
##Related Commands
*[Read-STFNetScalerConfiguration](Read-STFNetScalerConfiguration)
*[Wait-STFPublishServerGroupConfiguration](Wait-STFPublishServerGroupConfiguration)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.NetScalerConfigurationDocument
Parameter Configuration: The .NET 'Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.NetScalerConfigurationDocument' reference type
###System.Management.Automation.SwitchParameter
Parameter PropagateChanges: The .NET 'System.Management.Automation.SwitchParameter' value type
###Citrix.StoreFront.Model.Roaming.RoamingGateway[]
Parameter RoamingGatewaysToOverwrite: The .NET 'Citrix.StoreFront.Model.Roaming.RoamingGateway' reference type
###System.Management.Automation.SwitchParameter
Parameter CreateNew: The .NET 'System.Management.Automation.SwitchParameter' value type
###Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.ImportLogonType
Parameter LogonType: The .NET 'Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.ImportLogonType' value type
###System.String
Parameter CallbackUrl: The .NET 'System.String' reference type
###System.Int32
Parameter GatewayIndex: The .NET 'System.Int32' value type
##Return Values
###DocumentValidation
The .NET 'Citrix.StoreFront.Model.Roaming.NetScalerConfiguration.DocumentValidation' reference type
##Notes
-WhatIf parameter can be used to verify the configuration consistency.
##Examples
###EXAMPLE 1 Import a NetScaler remote access configuration
```
$stasToUpdate = Test-STFSecureTicketAuthority -StaConfigurationObject $netscalerConfiguration
Import-STFNetScalerConfiguration -Configuration $netscalerConfiguration
```
REMAR
```




The example reads in a NetScaler configuration package, validates that the Secure Ticket Authorities can be resolved 
and imports the configuration.

If validation errors are found they are output to the pipeline. If propagating to the cluster the progress can be 
monitored with Wait-STFPublishServerGroupConfiguration
```
###EXAMPLE 2 Import specific vServer from NetScaler remote access configuration file.
```
Import-STFNetScalerConfiguration -Configuration $ImportedGateways -GatewayIndex 0
Import-STFNetScalerConfiguration -Configuration $ImportedGateways -GatewayIndex 1
Import-STFNetScalerConfiguration -Configuration $ImportedGateways -GatewayIndex 2
```
REMARKS
The example reads in a NetScaler configuration package and then imports the first gateway defined in the package,
followed by the second and the third.
