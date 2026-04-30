---
title: "ChnRelativeHumidity"
description: "Calculates relative humidity from absolute humidity and temperature."
---

# ChnRelativeHumidity

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRelativeHumidity

Calculates relative humidity from absolute humidity and temperature.

## Signature

```python
return_value = dd.ChnRelativeHumidity( Y , Y , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the absolute humidity values. If you calculate in the quantity-based mode, DIAdem assumes that the absolute humidity is in g/m³. If you calculate in the quantity-based mode, DIAdem uses the channel unit.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the temperature values. If you do not calculate in the quantity-based mode, DIAdem assumes that the temperatures are in Kelvin. If you calculate in the quantity-based mode, DIAdem uses the channel unit.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel with the relative humidity in %. If you do not specify the name, DIAdem creates the <span class="Monospace">RelativeHumidity</span> channel in the default group. DIAdem overwrites an existing channel with the same name.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Specifies the result channel with the relative humidity . <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnRelativeHumidity.htm`*
