---
title: "ValMin"
description: "Determines the smaller of two numbers."
---

# ValMin

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ValMin

Determines the smaller of two numbers.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You must use the <a href="../calculate/">Calculate</a> command in scripts to calculate data channels with formulas. Compute the data channels according to the syntax in the Calculator. Refer to the procedures <a href="#" data-unresolved="1">Executing Channel Calculations in the Calculator</a> and <a href="#" data-unresolved="1">Assigning a Value to a Variable in the Calculator</a> for more information about the Calculator. Use the <a href="#" data-unresolved="1">MinV</a> command instead of <span class="Monospace">ValMin</span> when you calculate <a href="../../../varoff/variables/calcquantitybased/">quantity-based</a>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Value</td>
<td>Specifies the first numeric value.<div id="exp_Value">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">Value</td>
<td>Specifies the second numeric value.<div id="exp_Value__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number</a> type.</td></tr>
</table>
</div>

## Python example

```python
import math
MyValue1 = math.pi
MyValue2 = math.e
intMyResult = dd.ValMin(MyValue1,MyValue2) #intMyResult = 2.71828182845905
```

```python
dd.Calculate ("Ch(\"Group2/Result\")= ValMin (Ch(\"Group1/Input\"),Ch(\"Group1/Reference\"))")
```

---

*Source: `ComOff/ValMin.htm`*
