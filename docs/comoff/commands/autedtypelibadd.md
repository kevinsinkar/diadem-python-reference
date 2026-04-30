---
title: "AutEdTypeLibAdd"
description: "Registers a type library to be used in scripts."
---

# AutEdTypeLibAdd

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdTypeLibAdd

Registers a type library to be used in scripts.

## Signature

```python
dd.AutEdTypeLibAdd(AutEdTypeLibId, AutEdTypeLibVer)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>To copy the variables of the <span class="Monospace">AutEdTypeLibAdd</span> command to the clipboard, call the <a href="../autedtypelibdlg/">AutEdTypeLibDlg</a> command. Select a library and click <strong>Copy</strong>.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you specify the complete path in the <a href="../../../varoff/variables/autedtypelibid/">AutEdTypeLibId</a> variable, you do not need to specify the version.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>To copy the variables of the <span class="Monospace">AutEdTypeLibAdd</span> command to the clipboard, call the <a href="../autedtypelibdlg/">AutEdTypeLibDlg</a> command. Select a library and click <strong>Copy</strong>.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You can copy the variables for the <a href="./">AutEdTypeLibAdd</a> command to the clipboard if you open the <a href="#" data-unresolved="1">Registered Type Library</a> dialog box, specify a type library, and click <strong>Copy</strong>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  If you want to use a type library in a script, the file must be on the computer and registered in the operating system.  </td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AutEdTypeLibId</td>
<td>Specifies the identification of the type library you register in DIAdem.<div id="exp_AutEdTypeLibId">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>You can specify the type library either with the ID or with the complete path, for example, <span class="Monospace">AutEdTypeLibId = C:\WINDOWS\system32\scrrun.dll</span>.<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>To copy the variables of the <span class="Monospace">AutEdTypeLibAdd</span> command to the clipboard, call the <a href="../autedtypelibdlg/">AutEdTypeLibDlg</a> command. Select a library and click <strong>Copy</strong>.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">AutEdTypeLibVer</td>
<td>Specifies the type library version you register in DIAdem.<div id="exp_AutEdTypeLibVer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 255 characters</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you specify the complete path in the <a href="../../../varoff/variables/autedtypelibid/">AutEdTypeLibId</a> variable, you do not need to specify the version.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>To copy the variables of the <span class="Monospace">AutEdTypeLibAdd</span> command to the clipboard, call the <a href="../autedtypelibdlg/">AutEdTypeLibDlg</a> command. Select a library and click <strong>Copy</strong>.</td>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
# Microsoft Scripting Runtime
# C:\WINDOWS\system32\scrrun.dll
dd.AutEdTypeLibAdd("420B2830-E718-11CF-893D-00A0C9054228", "1.0")
dd.MsgBoxDisp("Constant ForWriting= " + ForWriting) # ForWriting = 2
```

```python
# Microsoft Scripting Runtime
dd.AutEdTypeLibAdd("C:\\WINDOWS\\system32\\scrrun.dll")
dd.MsgBoxDisp("Constant ForWriting= " + ForWriting) # ForWriting = 2
```

---

*Source: `ComOff/AutEdTypeLibAdd.htm`*
