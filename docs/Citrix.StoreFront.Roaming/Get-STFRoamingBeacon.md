#Get-STFRoamingBeacon
Get roaming beacons
##Syntax
```
Get-STFRoamingBeacon [-External] <SwitchParameter> [[-RoamingService] <RoamingService>] [<CommonParameters>]
```
##Detailed Description
Get the roaming beacons configured for the deployment.
##Related Commands
*[Set-STFRoamingBeacon](Set-STFRoamingBeacon)
*[Clear-STFRoamingBeacon](Clear-STFRoamingBeacon)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.Management.Automation.SwitchParameter
Parameter Internal: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter External: The .NET 'System.Management.Automation.SwitchParameter' value type
###Citrix.StoreFront.Model.Roaming.RoamingService
Parameter RoamingService: A .NET class representing the configuration of a StoreFront Roaming service
##Return Values
###String
The .NET 'System.String' reference type
##Examples
###EXAMPLE 1 Get internal beacon
```
```
REMARKS
Gets the internal beacon

```
```
REMARKS
Gets the external beacons
