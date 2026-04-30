---
title: "ChnEnvelopes"
description: "Calculates the upper and lower envelope curve of a signal."
---

# ChnEnvelopes

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEnvelopes

Calculates the upper and lower envelope curve of a signal.

## Signature

```python
return_value = dd.ChnEnvelopes( XW , Y , ResultChannel , ResultChannel , ResultChannel , ResultChannel , DXPeak)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If there are no extreme values in an interval, DIAdem uses each curve point as a data point of the envelope curve regardless of the interval width.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the envelope curve.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the upper envelope curve.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the lower envelope curve.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the lower envelope curve.</td></tr>
<tr><td width="150">DXPeak</td>
<td>Specifies the interval width as a percentage of the x-range in which DIAdem determines the extreme values.<div id="exp_DXPeak">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1E-9 &lt;= DXPeak &lt;= 100</td></tr>
</table>
<p class="Body">The interval width specifies how closely the envelope curve follows the original curve path. DIAdem determines the interpolation points of the envelope curve over the extreme values within the specified interval. DIAdem selects the interval point that has the maximum slope as the interpolation point for the envelope curve. This point is then the starting point for the next interval that is checked. The interval width must be greater than 0</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnEnvelopes.htm`*
