#Set-STFExplicitAuthenticator
Sets the password validator
##Syntax
```
Set-STFExplicitAuthenticator [-AuthenticationService <AuthenticationService>] [-Name <String>] [-AuthenticationService] <AuthenticationService> [[-DefaultManagerFactory] <SwitchParameter>] [[-Name] <String>] [<CommonParameters>]
```
##Detailed Description
Sets the password validator used for explicit configuration.
##Related Commands
*[Get-STFExplicitAuthenticator](Get-STFExplicitAuthenticator)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.Management.Automation.SwitchParameter
Parameter DefaultManagerFactory: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.String
Parameter Name: The .NET 'System.String' reference type
##Return Values
##Examples
###EXAMPLE 1 Set Password Validator
```
Set-STFExplicitAuthenticator -AuthenticationService $auth -Name "xmlServiceAuthenticator"
```
REMARKS
Configure the single authentication service to use the XmlService authenticator for explict authentication.

```
Set-STFExplicitAuthenticator -AuthenticationService $auth -DefaultManagerFactory
```
REMARKS
Configure the single authentication service to use the default authenticator for explict authentication.
