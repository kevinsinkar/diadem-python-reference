---
title: "IEMail.Send"
description: "Sends a mail you created in the EMail object."
---

# IEMail.Send

!!! abstract "Method &middot; `EMailService.chm`"
    Method: Send for EMail

Sends a mail you created in the EMail object.

## Signature

```python
obj.Send
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

*Source: `EMailService/methods/EMailService_method_Send_IEMail.htm`*
