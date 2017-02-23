#Set-STFStoreEnumerationOptions
Set Store enumeration options
##Syntax
```
```
##Detailed Description
Set the Store options used when enumerating the XenApp and XenDesktop xml services.
##Related Commands
*[Get-STFStoreEnumerationOptions](Get-STFStoreEnumerationOptions)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.Boolean
Parameter EnhancedEnumeration: The .NET 'System.Boolean' value type
###System.Int32
Parameter MaximumConcurrentEnumerations: The .NET 'System.Int32' value type
###System.String[]
Parameter FilterByTypesInclude: The .NET 'System.String' reference type
###System.String[]
Parameter FilterByKeywordsInclude: The .NET 'System.String' reference type
###System.String[]
Parameter FilterByKeywordsExclude: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.RequestFullIconData
Parameter RequestFullIconData: The .NET 'Citrix.StoreFront.Model.Store.RequestFullIconData' value type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Examples
###EXAMPLE 1 Turn off enhanced enumeration options
```
Set-STFStoreEnumerationOptions $storeService -EnhancedEnumeration $false
```
REMARKS
Turn off parallel enumeration of Store famrs.

```
Set-STFStoreEnumerationOptions $storeService -FilterByTypesInclude Applications
```
REMARKS
Filter resources to only show applications.

```
Set-STFStoreEnumerationOptions $storeService -FilterByKeywordsInclude AppSet1,AppSet2
```
REMARKS
Only publish resources in the Store that have the keywords AppSet1 or Appset2.

```
Set-STFStoreEnumerationOptions $storeService -FilterByKeywordsExclude AppSet1,AppSet2
```
REMARKS
Exclude resources from the store that have the keywords AppSet1 or Appset2
