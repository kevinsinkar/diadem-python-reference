---
title: "ADMCreateRight"
description: "Creates a new access right for the user management."
---

# ADMCreateRight

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ADMCreateRight

Creates a new access right for the user management.

## Signature

```python
dd.ADMCreateRight(ADMRight, ADMDescription)
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
<tr><td width="150">ADMDescription</td>
<td>Describes a user right.<div id="exp_ADMDescription">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 84 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
ADMRighADMRight = "Master"
ADMDescription = "Master rights"
ADMCreateRight(ADMRight, ADMDescription)
AskAdmPermission("Master")
if AdmPermission :
    dd.MsgBoxDisp("Allowed")
else:
    dd.MsgBoxDisp("Forbidden")
```

---

*Source: `ComOnl/ADMCreateRight.htm`*
