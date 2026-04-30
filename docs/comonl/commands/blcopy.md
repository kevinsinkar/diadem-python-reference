---
title: "BlCopy"
description: "Duplicates a DAC block in the current block diagram."
---

# BlCopy

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: BlCopy

Duplicates a DAC block in the current block diagram.

## Signature

```python
dd.BlCopy(BlName)
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

*Source: `ComOnl/BlCopy.htm`*
