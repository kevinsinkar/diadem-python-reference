---
title: "ChnLinGen"
description: "Generates a data channel with equidistant values."
---

# ChnLinGen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnLinGen

Generates a data channel with equidistant values.

## Signature

```python
return_value = dd.ChnLinGen( ResultChannel , GenXBegin, GenXEnd, XNo, [GenXUnitPreset])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">GenXBegin</td>
<td>Specifies the first value in a new data channel.<div id="exp_GenXBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">GenXEnd</td>
<td>Specifies the last value in a new data channel.<div id="exp_GenXEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XNo</td>
<td>Specifies the number of values in a new data channel.<div id="exp_XNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= XNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">[GenXUnitPreset]</td>
<td>Specifies the unit in which DIAdem generates the numeric channel. By default DIAdem does not use a unit. <div id="exp_GenXUnitPreset">
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
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
MyChnName = dd.ChnLinGen("Group/Channel3",0,100,201)
```

---

*Source: `ComOff/ChnLinGen.htm`*
