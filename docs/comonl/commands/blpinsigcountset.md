---
title: "BlPinSigCountSet"
description: "Specifies the number of terminals at inputs and outputs on DAC blocks and subblock diagrams."
---

# BlPinSigCountSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: BlPinSigCountSet

Specifies the number of terminals at inputs and outputs on DAC blocks and subblock diagrams.

## Signature

```python
dd.BlPinSigCountSet(BlNewPinSigCount)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BlNewPinSigCount</td>
<td>Specifies the list length of the open block terminal.<div id="exp_BlNewPinSigCount">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>1 &lt;= BlNewPinSigCount &lt;= <a href="../../../varonl/variables/blsignallistlength/">BlSignalListLength</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DACObjOpen("Input1")
dd.DACObjOpen("Data input")
dd.BlPinSigCountSet(11)
dd.DACObjClose("Data input")
dd.DACObjClose("Input1")
```

---

*Source: `ComOnl/BlPinSigCountSet.htm`*
