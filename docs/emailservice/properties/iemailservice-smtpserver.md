---
title: "IEMailService.SMTPServer"
description: "Specifies the internet address of the mail server over which DIAdem sends an email. You can specify the internet address as name or IP address. Most public mail"
---

# IEMailService.SMTPServer

!!! abstract "Property &middot; `EMailService.chm`"
    Property: SMTPServer for EMailService

Specifies the internet address of the mail server over which DIAdem sends an email. You can specify the internet address as name or IP address. Most public mail servers require a password and either an Email address or a user name as authentication.

## Signature

```python
obj.SMTPServer
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyEMailService.AccountEMailAddress = "john.doe@example.com"
oMyEMailService.AccountUserName = "john.doe@example.com"
oMyEMailService.AccountPassword = "secret_password"
oMyEMailService.SMTPTimeout = 30
oMyEMailService.SMTPServerPort = 465
oMyEMailService.SMTPUseSSL = True
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/properties/EMailService_property_SMTPServer_IEMailService.htm`*
