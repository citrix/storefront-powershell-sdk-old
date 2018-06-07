#Set-STFAccountSelfService
Sets Account self-service options
##Syntax
```
```
##Detailed Description
Sets the options of the Account self-service on a given Authentication service.
##Related Commands
*[Get-STFAccountSelfService](Get-STFAccountSelfService)
*[Get-STFAuthenticationServicePasswordManagerAccountSelfService](Get-STFAuthenticationServicePasswordManagerAccountSelfService)
*[Set-STFAuthenticationServicePasswordManagerAccountSelfService](Set-STFAuthenticationServicePasswordManagerAccountSelfService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.String
Parameter ManagerFactoryName: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter DefaultManagerFactory: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Boolean
Parameter AllowResetPassword: The .NET 'System.Boolean' value type
###System.Boolean
Parameter AllowUnlockAccount: The .NET 'System.Boolean' value type
##Return Values
##Examples
###EXAMPLE 1 Configure Account Self-Service
```
Set-STFAuthenticationServiceAccountSelfService -AuthenticationService $auth
```
REMARKS
Configure the single authentication service to use Account self-service 'passwordManagerSelfServiceAccountManagement'
factory.

```
Set-STFAuthenticationServiceAccountSelfService -AuthenticationService $auth -DefaultManagerFactory
```
REMARKS
Configure the single authentication service to not use account self-service.
