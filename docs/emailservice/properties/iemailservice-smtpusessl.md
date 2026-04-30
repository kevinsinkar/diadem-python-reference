---
title: "IEMailService.SMTPUseSSL"
description: "Specifies whether the mail server sends an email that is SSL encrypted."
---

# IEMailService.SMTPUseSSL

!!! abstract "Property &middot; `EMailService.chm`"
    Property: SMTPUseSSL for EMailService

Specifies whether the mail server sends an email that is SSL encrypted.

## Signature

```python
obj.SMTPUseSSL
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

*Source: `EMailService/properties/EMailService_property_SMTPUseSSL_IEMailService.htm`*
