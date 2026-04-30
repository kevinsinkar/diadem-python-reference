---
title: "GlobalDim"
description: "Declares global variables and reserves memory space for these variables. Global variables are valid and retain their contents as long as DIAdem is running and y"
---

# GlobalDim

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GlobalDim

Declares global variables and reserves memory space for these variables. Global variables are valid and retain their contents as long as DIAdem is running and you do not restart the script engine.

## Signature

```python
dd.GlobalDim(VarName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To delete global variables, you must restart the script engine with the <a href="../scriptcmdreset/">ScriptCmdReset</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You also can define global variables in user command files. Declare the variable in the global range outside a function and <a href="#" data-unresolved="1">register this user command file</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../globalredim/">GlobalRedim</a> command to declare global dynamic arrays.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use <a href="../iteminfoget/">ItemInfoGet</a> to check whether the variable already exists and whether the GlobalDim commands has executed it.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">VarName</td>
<td>Specifies the name of a global variable.<div id="exp_VarName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if not Iteminfoget("MyVar"):
    GlobalDim("MyVar, MyArray()")
```

---

*Source: `ComOff/GlobalDim.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
