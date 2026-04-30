---
title: "AskADMPermRt"
description: "Checks the access rights of the current user."
---

# AskADMPermRt

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: AskADMPermRt

Checks the access rights of the current user.

## Signature

```python
dd.AskADMPermRt(ADMRight)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Unlike the <a href="../askadmpermission/">AskADMPermission</a> command, DIAdem does not open the login dialog box if the user does not have the required rights.</td></tr></table>
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
<tr><td width="150">ADMPermission</td><td>Receives the check results.<div id="exp_ADMPermission__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-32000 &lt;= ADMPermission &lt;= 32000</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/AskADMPermRt.htm`*
