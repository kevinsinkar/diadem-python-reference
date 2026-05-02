---
title: "ScriptCMDRegister"
description: "Allows CodeCompletion for encrypted user commands. DIAdem takes the information for CodeCompletion from the TLB file."
---

# ScriptCMDRegister

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ScriptCMDRegister

Allows CodeCompletion for encrypted user commands. DIAdem takes the information for CodeCompletion from the TLB file.

## Signature

```python
dd.ScriptCMDRegister(ScriptCMDItemName, ScriptCMDTypeLibName, ScriptCMDInterfaceName)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ScriptCMDItemName</td>
<td>Specifies the name of the function or variable that was registered as user command or with the <span class="Monospace">GlobDim</span> command.<div id="exp_ScriptCMDItemName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ScriptCMDTypeLibName</td>
<td>Specifies the filename of a TLB file. You can enter the file with the absolute path or a filename. If you do not specify a path, DIAdem expects the file to be in the program directory.<div id="exp_ScriptCMDTypeLibName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ScriptCMDInterfaceName</td>
<td>Specifies the name of the interface for which DIAdem displays CodeCompletion.<div id="exp_ScriptCMDInterfaceName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
# Create global Variable
# Create instance of VBS class and assign to variable
GlobalTestObject = new MyTestClass

# Register typelib for test class
ScriptCMDRegister("GlobalTestObject",dd.ProgramDrv + "Examples\Documents\CMD_register.tlb", "TestTypelib.IMyTestClass")

# VBS Class
Class MyTestClass
m_SubClass = new MySubTestClass
m_PropValue = "Hello"

m_SubClass = None

SubClass = m_SubClass
End Property

MyTestProp = m_PropValue
End Property

m_PropValue = newValue
End Property

dd.MsgBox Param1 + Param2

End class

# VBS Sub Class
Class MySubTestClass
dd.MsgBox "Hi"
End Class
```

---

*Source: `ComOff/ScriptCMDRegister.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
