---
title: "IEMail.To"
description: "Specifies the email addresses to which DIAdem sends the email."
---

# IEMail.To

!!! abstract "Property &middot; `EMailService.chm`"
    Property: To for EMail

Specifies the email addresses to which DIAdem sends the email.

## Signature

```python
obj.To
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "", "This is the subject", "This is some text")
oMyMail.To       = "to@example.com"
oMyMail.BCC      = "blind.cc@example.com"
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/properties/EMailService_property_To_IEMail.htm`*
