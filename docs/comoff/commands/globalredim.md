---
title: "GlobalReDim"
description: "Declares global dynamic array variables and reserves memory space. Global variables are valid and retain their contents as long as DIAdem is running and you do "
---

# GlobalReDim

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GlobalReDim

Declares global dynamic array variables and reserves memory space. Global variables are valid and retain their contents as long as DIAdem is running and you do not restart the script engine.

## Signature

```python
dd.GlobalReDim(VarName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  To delete global variables, you must restart the script engine with the <a href="../scriptcmdreset/">ScriptCmdReset</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You also can define global variables in user command files. Declare the variable in the global range outside a function and <a href="#" data-unresolved="1">register this user command file</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../globaldim/">GlobalDim</a> command to define global variables.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The input parameters of the <span class="Monospace">GlobalReDim</span> command correspond to the arguments of the VBS function <a href="#" data-unresolved="1">ReDim</a>. Therefore, you can use the <span class="Monospace">Preserve</span> argument to get the data of the array when you modify the value of the dimension.</td></tr></table>
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
GlobalDim("MyVar, MyArray()")
GlobalReDim("MyArray(100)")
```

```python
ScriptCmdReset
GlobalDim "MyArray()"
GlobalReDim "MyArray(3)"
for iCount in range(0, Ubound(MyArray) + 1):
    MyArray(iCount)=iCount
GlobalRedim "Preserve MyArray(2)"
for iCount in range(0, Ubound(MyArray) + 1):
    MsgBoxDisp (MyArray(iCount))
```

---

*Source: `ComOff/GlobalReDim.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
