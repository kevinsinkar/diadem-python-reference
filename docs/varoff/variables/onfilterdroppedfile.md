---
title: "OnFilterDroppedFile"
description: "Specifies the user command that DIAdem executes when you drag and drop one or more files onto DIAdem. DIAdem does not execute this function when you drag the fi"
---

# OnFilterDroppedFile

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: OnFilterDroppedFile

Specifies the user command that DIAdem executes when you drag and drop one or more files onto DIAdem. DIAdem does not execute this function when you drag the files onto DIAdem SCRIPT. You cannot assign several user commands to the OnFilterDroppedFile event.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Panel</td>
<td>Specifies the name of the panel onto which you dragged a file.<br attr="ext"/><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr><td width="150">FileName</td>
<td>Specifies the name of the file that you dragged onto DIAdem.<br attr="ext"/><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr><td width="150">Reserved</td>
<td>For future extensions. Always contains the value <a href="#" data-unresolved="1">Zero</a>.<br attr="ext"/><a href="#" data-unresolved="1">Variant variable</a></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. If the value is <span class="Monospace">TRUE</span>, DIAdem does not continue processing the dragged file. If the value is <span class="Monospace">FALSE</span>, the dragged value is forwarded to DIAdem and the default action is executed.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
OnFilterDroppedFile = "MyOnFilterDroppedFile"

def MyOnFilterDroppedFile(Panel, FileName, Reserved):
    LogfileWrite("Execute OnFilterDroppedFile: Panel: " + Panel + "\r\n" + "Filename " + FileName)
    if (UpC(NameSplit(Filename, "E")) == "TXT"):
        MyOnFilterDroppedFile = False  # True
        # do something
    else:
        MyOnFilterDroppedFile = False  # True
        # do something else
```

---

*Source: `VarOff/OnFilterDroppedFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
