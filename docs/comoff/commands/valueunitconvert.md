---
title: "ValueUnitConvert"
description: "Converts a numeric value from one unit to a different unit."
---

# ValueUnitConvert

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ValueUnitConvert

Converts a numeric value from one unit to a different unit.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ValueUnit</td>
<td>Specifies the numeric value of which DIAdem converts the unit.<div id="exp_ValueUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SourceUnit</td>
<td>Specifies the symbol of the source unit.<div id="exp_SourceUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TargetUnit</td>
<td>Specifies the symbol of the target unit.<div id="exp_TargetUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number variable</a> type. Receives the value in the converted unit.</td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.ValueUnitConvert(1,"m","in"))
```

---

*Source: `ComOff/ValueUnitConvert.htm`*
