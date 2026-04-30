---
title: "ChnGeoGen"
description: "Generates a data channel with geometric partitions."
---

# ChnGeoGen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGeoGen

Generates a data channel with geometric partitions.

## Signature

```python
return_value = dd.ChnGeoGen( ResultChannel , GenXBegin, GenXEnd, XNo, [GenXUnitPreset])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">GenXBegin</span> variable and the <span class="Monospace">GenXEnd</span> variable must have the same sign.</td></tr></table>
</div>

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
MyChnName = dd.ChnGeoGen("Group/Channel3",1,2048,12)
```

---

*Source: `ComOff/ChnGeoGen.htm`*
