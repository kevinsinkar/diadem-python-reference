---
title: "IEMail.From"
description: "Specifies the email address of the sender. If you want to include the name in the email address, enter the actual email address between < and > characters."
---

# IEMail.From

!!! abstract "Property &middot; `EMailService.chm`"
    Property: From for EMail

Specifies the email address of the sender. If you want to include the name in the email address, enter the actual email address between < and > characters.

## Signature

```python
obj.From
```

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.From     = "from.example@example.com"
oMyMail.Send()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/properties/EMailService_property_From_IEMail.htm`*
