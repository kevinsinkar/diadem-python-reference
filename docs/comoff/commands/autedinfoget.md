---
title: "AutEdInfoGet"
description: "Provides information about the files loaded in the script editor and the modification status of the files."
---

# AutEdInfoGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdInfoGet

Provides information about the files loaded in the script editor and the modification status of the files.

## Signature

```python
dd.AutEdInfoGet()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AutEdExt</td><td>Specifies the filename extension of the file enabled in the script editor.<div id="exp_AutEdExt">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdName</td><td>Specifies the name of the file enabled in the script editor.<div id="exp_AutEdName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoFiles</td><td>Specifies the number of files open in the script editor.<div id="exp_AutEdNoFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoVBSFiles</td><td>Specifies the number of VBS files open in the script editor.<div id="exp_AutEdNoVBSFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoAUTFiles</td><td>Specifies the number of AUT files open in the script editor.<div id="exp_AutEdNoAUTFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoVASFiles</td><td>Specifies the number of VAS files open in the script editor.<div id="exp_AutEdNoVASFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoLSTFiles</td><td>Specifies the number of LST files open in the script editor.<div id="exp_AutEdNoLSTFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoASCFiles</td><td>Specifies the number of ASC files open in the script editor.<div id="exp_AutEdNoASCFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdNoElseFiles</td><td>Specifies the number of other files open in the script editor.<div id="exp_AutEdNoElseFiles">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdModifiedIs</td><td>Specifies whether the file enabled in the script editor was changed.<div id="exp_AutEdModifiedIs">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.AutEdInfoGet()
strMsg = "List of opened files: " + "\r\n"
for iLoop in range( 0, dd.AutEdNoFiles - 1+1):
    dd.AutEdTabNameGet(iLoop)
    strMsg = strMsg + dd.AutEdTabName + "\r\n"
dd.MsgBoxDisp(strMsg)
```

---

*Source: `ComOff/AutEdInfoGet.htm`*
