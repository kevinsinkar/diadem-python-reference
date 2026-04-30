---
title: "AutEdFileOpen"
description: "Opens a file in the script editor."
---

# AutEdFileOpen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdFileOpen

Opens a file in the script editor.

## Signature

```python
dd.AutEdFileOpen(FileDlgName, [AutEdSyntax])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path in the <span class="Monospace">FileDlgName</span> variable, DIAdem loads the file from the SCRIPT user folder or saves the file in the SCRIPT user folder. If you do not enter a filename extension, DIAdem determines the filename extension from the variable <a href="../../../varoff/variables/filedlgfilt/">FileDlgFilt</a>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileDlgName</td>
<td>Specifies a file. You can also specify the path and the filename extension.<div id="exp_FileDlgName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path in the <span class="Monospace">FileDlgName</span> variable, DIAdem loads the file from the SCRIPT user folder or saves the file in the SCRIPT user folder. If you do not enter a filename extension, DIAdem determines the filename extension from the variable <a href="../../../varoff/variables/filedlgfilt/">FileDlgFilt</a>.</td></tr></table>
</div></td></tr>
<tr><td width="150">[AutEdSyntax]</td>
<td>Specifies the syntax of the loaded file.<div id="exp_AutEdSyntax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p>Possible values are:</p>
<table class="Borderless"><tr><td width="150">VBS DIADEM</td><td>Uses the syntax support for DIAdem VBS scripts in the script editor.</td></tr><tr><td width="150">VBS-DATA-PLUGIN</td><td>Uses the syntax support for DataPlugin scripts in the script editor.</td></tr></table>
<p>If you do not specify a value, DIAdem uses the value <span class="Monospace">VBS DIADEM</span>.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AutEdFileOpen.htm`*
