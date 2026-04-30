---
title: "IEMailService.AccountPassword"
description: "Specifies the password of the sender for authentication at the mail server. Most public mail servers require authentication with a password or an email address "
---

# IEMailService.AccountPassword

!!! abstract "Property &middot; `EMailService.chm`"
    Property: AccountPassword for EMailService

Specifies the password of the sender for authentication at the mail server. Most public mail servers require authentication with a password or an email address or a user name .

## Signature

```python
obj.AccountPassword
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

*Source: `EMailService/properties/EMailService_property_AccountPassword_IEMailService.htm`*
