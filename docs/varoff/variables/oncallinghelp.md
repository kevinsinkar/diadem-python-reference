---
title: "OnCallingHelp"
description: "Specifies which user command DIAdem executes when the Help is called."
---

# OnCallingHelp

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: OnCallingHelp

Specifies which user command DIAdem executes when the Help is called.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The user command is not executed if you select a term in DIAdem SCIRPT and call the context help with the <span class="Monospace">F1</span> function key.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150">ContextObject</td>
<td>Specifies the Context object. The Context object has three properties.<br attr="ext"/>
<table class="Borderless">
<tr>
<td width="150"><donottranslate>FileName</donottranslate></td>
<td>Specifies the name of the help file. When the help call calls DIAdem help, this property contains the value <span class="Monospace">"DIADEM.CHM"</span>.<br attr="ext"/><a href="#" data-unresolved="1">String variable</a></td>
</tr>
<tr>
<td width="150"><donottranslate>Topic</donottranslate></td>
<td>Contains the unique name of the called help page.<br attr="ext"/><a href="#" data-unresolved="1">String variable</a></td>
</tr>
<tr>
<td width="150"><donottranslate>DoProceed</donottranslate></td>
<td>Specifies whether DIAdem calls the user command which calls the DIAdem help (TRUE) or not (FALSE).<br attr="ext"/>Boolean with read and write access</td>
</tr>
</table>
</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
OnCallingHelp = "MyOnHelp"

def MyOnHelp(Context):
    LogfileWrite(Context.Filename + "\t" &Context.Topic + "\t" + Context.DoProceed)
    if (Context.Topic == "GENREPORT_OVERVIEW"):
        CustomHelpShow("Customize.chm", "Customize.chm::/report.htm")
        Context.DoProceed = False
    else:
        Context.DoProceed = True
```

---

*Source: `VarOff/OnCallingHelp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
