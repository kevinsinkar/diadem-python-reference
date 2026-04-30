---
title: "IEMailService"
description: "The EMailService object connects to the mail server and provides the mail server with the necessary properties. Use the CreateEMailService command to create the"
---

# IEMailService

!!! abstract "Object &middot; `EMailService.chm`"
    Object: EMailService

The EMailService object connects to the mail server and provides the mail server with the necessary properties. Use the CreateEMailService command to create the EMailService object. The EMailService object does not support servers which demand STARTTLS. Note The objects EMailService and EMail are only available in the 64-bit version of DIAdem.

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
<p><a href="../../properties/iemailservice-accountemailaddress/">AccountEMailAddress</a> | <a href="../../properties/iemailservice-accountpassword/">AccountPassword</a> | <a href="../../properties/iemailservice-accountusername/">AccountUserName</a> | <a href="../../properties/iemailservice-smtpserver/">SMTPServer</a> | <a href="../../properties/iemailservice-smtpserverport/">SMTPServerPort</a> | <a href="../../properties/iemailservice-smtptimeout/">SMTPTimeout</a> | <a href="../../properties/iemailservice-smtpusessl/">SMTPUseSSL</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iemailservice-createemail/">CreateEMail</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `EMailService/objects/EMailService_Objects_IEMailService.htm`*
