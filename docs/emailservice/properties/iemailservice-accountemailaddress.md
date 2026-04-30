---
title: "IEMailService.AccountEMailAddress"
description: "Specifies the email address of the sender for authentication at the mail server. Most public mail servers require a password and either an email address or a us"
---

# IEMailService.AccountEMailAddress

!!! abstract "Property &middot; `EMailService.chm`"
    Property: AccountEMailAddress for EMailService

Specifies the email address of the sender for authentication at the mail server. Most public mail servers require a password and either an email address or a user name as authentication. This email address does not appear as the sender in the created email. Use the From property to specify the return address of the email.

## Signature

```python
obj.AccountEMailAddress
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

*Source: `EMailService/properties/EMailService_property_AccountEMailAddress_IEMailService.htm`*
