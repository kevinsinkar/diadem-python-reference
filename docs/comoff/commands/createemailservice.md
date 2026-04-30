---
title: "CreateEMailService"
description: "Creates an EMailService object . The EMailService object connects to the mail server and provides the mail server with the necessary properties."
---

# CreateEMailService

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateEMailService

Creates an EMailService object . The EMailService object connects to the mail server and provides the mail server with the necessary properties.

## Signature

```python
return_value = dd.CreateEMailService( SMTPServerName )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SMTPServerName</td>
<td>Specifies the internet address of the mail server over which DIAdem sends an email. You can specify the internet address as name or IP address.<div id="exp_SMTPServerName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../emailservice/objects/iemailservice/">EMailService object</a> type.</td></tr>
</table>
</div>

## Python example

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.Send()
```

```python
oMyEMailService = dd.CreateEMailService("server.example.com")
oMyEMailService.AccountEMailAddress = "john.doe@example.com"
oMyEMailService.AccountUserName = "john.doe@example.com"
oMyEMailService.AccountPassword = "secret_password"
oMyEMailService.SMTPTimeout = 30
oMyEMailService.SMTPServerPort = 465
oMyEMailService.SMTPUseSSL = True
oMyMail = oMyEMailService.CreateEMail("FromUser <from.example@example.com>", "ToUser <to.example@example.com>", "This is the subject", "This is some text")
oMyMail.Send()
```

---

*Source: `ComOff/CreateEMailService.htm`*
