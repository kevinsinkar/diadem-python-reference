---
title: "IEMail.CC"
description: "Specifies the email addresses to which DIAdem sends an email copy. Separate several email addresses with a comma. If you want to include the name in the email a"
---

# IEMail.CC

!!! abstract "Property &middot; `EMailService.chm`"
    Property: CC for EMail

Specifies the email addresses to which DIAdem sends an email copy. Separate several email addresses with a comma. If you want to include the name in the email address, enter the actual email address between < and > characters.

## Signature

```python
obj.CC
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.CC       = "to.cc@example.com"
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

*Source: `EMailService/properties/EMailService_property_CC_IEMail.htm`*
