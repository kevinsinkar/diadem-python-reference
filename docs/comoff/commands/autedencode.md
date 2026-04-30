---
title: "AutEdEncode"
description: "Encrypts VBS files and SUD files."
---

# AutEdEncode

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdEncode

Encrypts VBS files and SUD files.

## Signature

```python
dd.AutEdEncode(CryptFile)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You also can select <strong>Script»Encrypt VBS script/SUD file</strong> to encrypt files in the DIAdem SCRIPT panel.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The encrypted files have the extensions <span class="Monospace">.vbc</span> and <span class="Monospace">.suc</span>. You cannot decrypt an encrypted file. If you specify a user dialog box file or a script file without a filename extension in order to display or to execute these scripts, DIAdem first searches for the unencrypted file with the filename extension <span class="Monospace">.sud</span> or <span class="Monospace">.vbs</span> and then searches for the encrypted file with the filename extension <span class="Monospace">.suc</span> or <span class="Monospace">.vbc</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CryptFile</td>
<td>Specifies which file to encrypt. You can also specify the path and the filename extension.<div id="exp_CryptFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AutEdEncode.htm`*
