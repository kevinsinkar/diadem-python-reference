---
title: "CreateValueWithUnit"
description: "Generates a ValueWithUnit object ."
---

# CreateValueWithUnit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateValueWithUnit

Generates a ValueWithUnit object .

## Signature

```python
return_value = dd.CreateValueWithUnit(oValue, UnitSymbol )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">oValue</td>
<td>Specifies the value of the quantity.<div id="exp_oValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">UnitSymbol</td>
<td>Specifies the unit of the quantity.<div id="exp_UnitSymbol">
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
<td>The return value is a <a href="../../../ivalueunit/objects/ivalueunit/">ValueWithUnit object</a> type.</td></tr>
</table>
</div>

## Python example

```python
MyValueUnit = dd.CreateValueWithUnit(0.61,"m")
MyValueUnit.Convert("in")
dd.MsgBoxDisp(MyValueUnit.Value)
```

---

*Source: `ComOff/CreateValueWithUnit.htm`*
