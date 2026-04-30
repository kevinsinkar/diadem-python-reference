---
title: "ChnSplitAtValue"
description: "Splits a channel into two new channels at a specified limit value."
---

# ChnSplitAtValue

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSplitAtValue

Splits a channel into two new channels at a specified limit value.

## Signature

```python
return_value = dd.ChnSplitAtValue( Y , SplitValue, FloorIsNovalue, ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values to be split.</td></tr>
<tr><td width="150">SplitValue</td>
<td>Specifies the limit value at which DIAdem splits a channel. The default setting is <span class="Monospace">0</span>.<div id="exp_SplitValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">FloorIsNovalue</td>
<td>Specifies whether DIAdem replaces the value that corresponds to the <span class="Monospace">SplitValue</span> variable with <span class="Monospace">NoValue</span> or with the value of the SplitValue variable, in the result channels.<div id="exp_FloorIsNovalue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the values above the limit value.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the values below the limit value.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnSplitAtValue.htm`*
