---
title: "AutEdSaveAsDlg"
description: "Opens the dialog box for saving files in the script editor, without saving the file."
---

# AutEdSaveAsDlg

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdSaveAsDlg

Opens the dialog box for saving files in the script editor, without saving the file.

## Signature

```python
dd.AutEdSaveAsDlg(FileDlgName)
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
</table>
</div>

## Python example

```python
dd.AutEdInfoGet()
dd.FileDlgName = dd.AutEdName
dd.AutEdSaveAsDlg(dd.FileDlgName)
intLoop = 0
if dd.DlgState == "IDOk" :
    dd.AutEdTabNameGet(intLoop)
    while (intLoop < dd.AutEdNoFiles and dd.AutEdTabName != dd.AutEdName):
        intLoop = intLoop +1
        dd.AutEdTabNameGet(intLoop)
    dd.AutEdTabSave(intLoop,dd.FileDlgName)
```

---

*Source: `ComOff/AutEdSaveAsDlg.htm`*
