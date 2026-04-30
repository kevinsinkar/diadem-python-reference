---
title: "IEMail.TextBody"
description: "Specifies the text of an email. The text can contain text but not formats."
---

# IEMail.TextBody

!!! abstract "Property &middot; `EMailService.chm`"
    Property: TextBody for EMail

Specifies the text of an email. The text can contain text but not formats.

## Signature

```python
obj.TextBody
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "")
oMyMail.TextBody = "Hello World" + "\r\n" + "This is my first email!"
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/properties/EMailService_property_TextBody_IEMail.htm`*
