---
title: "IEMailService.SMTPTimeout"
description: "Specifies the time in seconds that DIAdem needs to connect to the mail server."
---

# IEMailService.SMTPTimeout

!!! abstract "Property &middot; `EMailService.chm`"
    Property: SMTPTimeout for EMailService

Specifies the time in seconds that DIAdem needs to connect to the mail server.

## Signature

```python
obj.SMTPTimeout
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

*Source: `EMailService/properties/EMailService_property_SMTPTimeout_IEMailService.htm`*
