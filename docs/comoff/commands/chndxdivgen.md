---
title: "ChnDXDivGen"
description: "Generates a data channel by partitioning a specific x-channel into equidistant sections."
---

# ChnDXDivGen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDXDivGen

Generates a data channel by partitioning a specific x-channel into equidistant sections.

## Signature

```python
return_value = dd.ChnDXDivGen( X , ResultChannel , GenXBegin, GenXEnd, XDiv)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>When DIAdem executes this command, DIAdem does not include the variables <span class="Monospace">GenXBegin</span> and <span class="Monospace">GenXEnd</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
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
<tr><td width="150">XDiv</td>
<td>Specifies the number of equidistant sections in each interval of the x-range.<div id="exp_XDiv">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= XDiv &lt;= 100</td></tr>
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
MyChnName = dd.ChnDXDivGen("Group/Channel1","Group/Channel3",0,0,5)
```

---

*Source: `ComOff/ChnDXDivGen.htm`*
