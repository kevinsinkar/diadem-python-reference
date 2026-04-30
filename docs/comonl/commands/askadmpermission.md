---
title: "AskADMPermission"
description: "Checks the access rights of the current user and opens the dialog box for logging on if the user does not have the required rights."
---

# AskADMPermission

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: AskADMPermission

Checks the access rights of the current user and opens the dialog box for logging on if the user does not have the required rights.

## Signature

```python
dd.AskADMPermission(ADMRight)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to <a href="#" data-unresolved="1">User Management for DIAdem - General</a> for further information.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ADMRight</td>
<td>Specifies the name of a user right.<div id="exp_ADMRight">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 84 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ADMPermission</td><td>Receives the check results.<div id="exp_ADMPermission">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-32000 &lt;= ADMPermission &lt;= 32000</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
ADMRight = "Master"
ADMDescription = "Master rights"
ADMCreateRight(ADMRight, ADMDescription)
AskAdmPermission("Master")
if AdmPermission :
    dd.MsgBoxDisp("Allowed")
else:
    dd.MsgBoxDisp("Forbidden")
```

---

*Source: `ComOnl/AskADMPermission.htm`*
