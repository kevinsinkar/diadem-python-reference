---
title: "IEMailService.CreateEMail"
description: "Creates an EMail object containing an email to send over an email server. Use the Send method to send emails. Separate several email addresses with commas. If y"
---

# IEMailService.CreateEMail

!!! abstract "Method &middot; `EMailService.chm`"
    Method: CreateEMail for EMailService

Creates an EMail object containing an email to send over an email server. Use the Send method to send emails. Separate several email addresses with commas. If you want to include the name in the email address, enter the actual email address between < and > characters.

## Signature

```python
return_value = obj.CreateEMail(From, To, Subject, TextBody)
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
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

*Source: `EMailService/methods/EMailService_method_CreateEMail_IEMailService.htm`*
