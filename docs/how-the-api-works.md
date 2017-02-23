# How the API works




The location value in the challenge specifies a URL that the client requests (via Ajax) to determine which authentication methods are available. The challenge may contain an additional attribute `mode=Redirect`, which triggers the client to redirect to a 3rd party page instead to perform the authentication step.








|----------|-----------|----------|----------|-----------------------------------------------------|
| **ASP.NET_SessionId** | Session    | Yes | First response from Web Proxy | ASP.NET session id, represents the web session between client and Web Proxy.| 
| **CtxsAuthId** | Session | Yes | Response indicating successful authentication| Protects against session fixation attacks |
|**CsrfToken** | Session | No | First response from Web Proxy | Protects against cross- site request forgery attacks |
| **CtxsDeviceId** | Persistent, 2 years | Yes | Response indicating successful resource enumeration | Specifies the value to use for client name and device id (see above) |

## HTTPS indicator to secure cookies

```
application/x-www-form-urlencoded
```
