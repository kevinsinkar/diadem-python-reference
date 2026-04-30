---
title: "ChnOrdAFCalc"
description: "Calculates an order analysis in the frequency domain."
---

# ChnOrdAFCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnOrdAFCalc

Calculates an order analysis in the frequency domain.

## Signature

```python
dd.ChnOrdAFCalc( XW , Y , X1 )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem interprets the value of the variable <span class="Monospace">OrdAFMaxOrder</span> only if the variable <span class="Monospace">OrdAFType</span> has the value <span class="Monospace">Order</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../ordafparaset/">OrdAFParaSet</a> command to set the parameters for order analysis in the frequency domain according to the input channels.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values of the signal you want to analyze.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal you want to analyze.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the rpm values of the signal you want to analyze.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnOrdAFCalc.htm`*
