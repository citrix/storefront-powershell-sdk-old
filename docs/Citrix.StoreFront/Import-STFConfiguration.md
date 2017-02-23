#Import-STFConfiguration
Imports a zip file containing configuration elements that form a Citrix StoreFront deployment. This zip file may be unencrypted in the form of a '.zip' file or encrypted in the form of a '.ctxzip'.
##Syntax
```
```
##Detailed Description
Imports a zip file containing configuration elements that form a Citrix StoreFront deployment. This zip file may be unencrypted in the form of a '.zip' file or encrypted in the form of a '.ctxzip'.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter ConfigurationZip: The .NET 'System.String' reference type
###System.Management.Automation.PSCredential
Parameter Credential: The .NET 'System.Management.Automation.PSCredential' reference type
###System.String
Parameter HostBaseUrl: The .NET 'System.String' reference type
###System.Int64
Parameter SiteId: The .NET 'System.Int64' value type
##Return Values
##Examples
###EXAMPLE 1 Basic Config Import
```
```
REMARKS
This will import the ConfigBackup.zip configuration archive using the host base url and site id from the exported
configuration.

```
```
REMARKS
Using the password supplied in $CredObject this cmdlet will decrypt and import the ConfigBackup.ctxzip backup archive
using the host base url and site id from the exported configuration.
Example PSCredential:
$User = Any non empty string will suffice here. The exported configuration is secured by only using the $Password.
$Password = 'Secret'
$Password = $Password | ConvertTo-SecureString -asPlainText -Force
$CredObject = New-Object System.Management.Automation.PSCredential($User,$Password)
Create a PowerShell credential object containing a username and password for symmetric encryption and decryption of
configuration backup archives. PowerShell credential objects store passwords as secure strings in memory.
The user is irrelevant but mandatory to create a PowerShell credential object. The example code uses the currently
logged in user.
The password is used for symmetric encryption/decryption of the backup archive. NOTE: The password DOES NOT need to
match the user's password to create a valid credential object.
