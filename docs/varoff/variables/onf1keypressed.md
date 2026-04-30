---
title: "OnF1KeyPressed"
description: "Specifies the user command DIAdem executes when you press F1. DIAdem does not execute this function in a user dialog box. Instead use the EventFuncKeyPressed ev"
---

# OnF1KeyPressed

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: OnF1KeyPressed

Specifies the user command DIAdem executes when you press F1. DIAdem does not execute this function in a user dialog box. Instead use the EventFuncKeyPressed event in user dialog boxes. You cannot assign several user commands to the OnF1KeyPressed event.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>. Use the <a href="../../../comoff/commands/customhelpshow/">CustomHelpShow</a> command to call the user-defined help.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Panel</td>
<td>Specifies the name of the panel in which the F1 call is executed.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Variant variable</a></td>
</tr>
</table>
</td></tr>
<tr><td width="150">Reserved</td>
<td>For future extensions. Always contains the value <a href="#" data-unresolved="1">Zero</a>.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Variant variable</a></td>
</tr>
</table>
</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. If the value is <span class="Monospace">TRUE</span>, the F1 call is transferred to DIAdem and the respective DIAdem help is called. If the value is <span class="Monospace">FALSE</span>, the F1 call is not transferred to DIAdem.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
OnF1KeyPressed = "MyOnF1KeyPressed"

def MyOnF1KeyPressed(Panel, Reserved):
    MyOnF1KeyPressed = True
    # select Panel
    # case "VIEW"
    MyOnF1KeyPressed = FALSE
    # case "REPORT"
    CustomHelpShow("Customize.chm", "Customize.chm::/report.htm")
    MyOnF1KeyPressed = FALSE
    # case else
```

---

*Source: `VarOff/OnF1KeyPressed.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
