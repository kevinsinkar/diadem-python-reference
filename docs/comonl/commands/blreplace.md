---
title: "BlReplace"
description: "Replaces a DAC block with another similar DAC block in the current block diagram."
---

# BlReplace

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: BlReplace

Replaces a DAC block with another similar DAC block in the current block diagram.

## Signature

```python
dd.BlReplace(BlName, BlName)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BlName</td>
<td>Specifies the name of a DAC block.<div id="exp_BlName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 16 characters</td></tr>
</table>
</div></td></tr>
<tr><td width="150">BlName</td>
<td>Specifies the name of a DAC block.<div id="exp_BlName__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 16 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.BlCopy("Input1")
dd.DacObjOpen("Input2")
dd.DACObjRename("Input2","NIDAQ201")
dd.DacObjClose(dd.BlActName)
dd.BlReplace("Source","NIDAQ201")
```

---

*Source: `ComOnl/BlReplace.htm`*
