#Add-STFSessionManagerTrustedIssuer
Add a session manager trusted issuer to a store.
##Syntax
```
```
##Detailed Description
Adds a trusted issuer with a certificate thumbprint to indicate that SAML requests originating from a session manager that are signed by the certificate are to be trusted.
##Related Commands
*[Remove-STFSessionManagerTrustedIssuer](Remove-STFSessionManagerTrustedIssuer)
*[New-STFSessionManagerTrustedIssuer](New-STFSessionManagerTrustedIssuer)
*[Get-STFStoreService](Get-STFStoreService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###Citrix.StoreFront.Model.SessionManager.SessionManagerTrustedIssuer
Parameter SessionManagerTrustedIssuer: The .NET 'Citrix.StoreFront.Model.SessionManager.SessionManagerTrustedIssuer' reference type
##Return Values
##Examples
###EXAMPLE 1 Add a session manager trusted issuer to a store service.
```
$trustedIssuer = New-STFSessionManagerTrustedIssuer -Thumbprint '9ca5d6dbc06fc48cb0115d337c7b030aba56a835' -Name 'test issuer'
Add-STFSessionManagerTrustedIssuer -StoreService $storeService -SessionManagerTrustedIssuer $trustedIssuer
```
REMARKS
Add a session manager trusted issuer to a store service.
