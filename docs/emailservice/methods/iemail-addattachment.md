---
title: "IEMail.AddAttachment"
description: "Adds an attachment to an email. If you call the AddAttachment method several times, you can add several attachments."
---

# IEMail.AddAttachment

!!! abstract "Method &middot; `EMailService.chm`"
    Method: AddAttachment for EMail

Adds an attachment to an email. If you call the AddAttachment method several times, you can add several attachments.

## Signature

```python
obj.AddAttachment(Filename)
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text.")
oMyMail.AddAttachment("c:\\Attachment.txt")
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/methods/EMailService_method_AddAttachment_IEMail.htm`*
