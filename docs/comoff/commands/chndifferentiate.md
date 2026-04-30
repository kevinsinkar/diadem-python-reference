---
title: "ChnDifferentiate"
description: "Differentiates a signal numerically by calculating the forward difference quotient of the first order."
---

# ChnDifferentiate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDifferentiate

Differentiates a signal numerically by calculating the forward difference quotient of the first order.

## Signature

```python
return_value = dd.ChnDifferentiate( XW , Y , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the mean values of two successive x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel with the forward difference quotient.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnDifferentiate.htm`*
