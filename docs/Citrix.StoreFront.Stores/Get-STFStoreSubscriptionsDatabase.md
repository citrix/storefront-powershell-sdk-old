#Get-STFStoreSubscriptionsDatabase
Gets the location of the subscription data storage for the specified Store
##Syntax
```
```
##Detailed Description
Gets the connection string for the SQL Server database currently used for subscription data for the specified Store.
##Related Commands
*[Set-STFStoreSubscriptionsDatabase](Set-STFStoreSubscriptionsDatabase)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
##Return Values
###StoreSubscriptionDatabaseSummary
The .NET 'Citrix.StoreFront.Model.Store.Summary.StoreSubscriptionDatabaseSummary' reference type
##Examples
###EXAMPLE 1 Get the subscription database connection
```
Get-STFStoreStoreSubscriptionsDatabase -StoreService $store
```
REMARKS
Gets the subscription database connection for the only configured Store service.
OUTPUT
```
--------------- ------------------------
False           Server=myServerAddress;Database=myDataBase;User Id=myUsername;Password=myPassword;
```