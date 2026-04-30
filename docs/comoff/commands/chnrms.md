---
title: "ChnRMS"
description: "Calculates floating root mean squares, RMS."
---

# ChnRMS

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRMS

Calculates floating root mean squares, RMS.

## Signature

```python
return_value = dd.ChnRMS( XW , Y , ResultChannel , RMSWidth)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The x-values must be equidistant and strictly monotonic increasing.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">RMSWidth</td>
<td>Specifies how many neighboring values are included, as a percentage of the channel length. If there are less values at the boundaries, the calculation runs with less values at one end.<div id="exp_RMSWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1E-9 &lt;= RMSWidth &lt;= 100</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnRMS.htm`*
