---
title: "IEMail.Subject"
description: "Specifies the subject of an email."
---

# IEMail.Subject

!!! abstract "Property &middot; `EMailService.chm`"
    Property: Subject for EMail

Specifies the subject of an email.

## Signature

```python
obj.Subject
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "", "This is some text")
oMyMail.Subject = "This is the subject"
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/properties/EMailService_property_Subject_IEMail.htm`*
