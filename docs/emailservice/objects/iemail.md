---
title: "IEMail"
description: "The EMail object provides an email to send over an email server. Use the CreateEMail method to create the EMail object. Use the Send method to send emails. Note"
---

# IEMail

!!! abstract "Object &middot; `EMailService.chm`"
    Object: EMail

The EMail object provides an email to send over an email server. Use the CreateEMail method to create the EMail object. Use the Send method to send emails. Note The objects EMailService and EMail are only available in the 64-bit version of DIAdem.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The objects <strong>EMailService</strong> and <strong>EMail</strong> are only available in the 64-bit version of DIAdem.</td></tr></table>
</div>

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.Send()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iemail-bcc/">BCC</a> | <a href="../../properties/iemail-cc/">CC</a> | <a href="../../properties/iemail-from/">From</a> | <a href="../../properties/iemail-subject/">Subject</a> | <a href="../../properties/iemail-textbody/">TextBody</a> | <a href="../../properties/iemail-to/">To</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iemail-addattachment/">AddAttachment</a> | <a href="../../methods/iemail-send/">Send</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/objects/EMailService_Objects_IEMail.htm`*
