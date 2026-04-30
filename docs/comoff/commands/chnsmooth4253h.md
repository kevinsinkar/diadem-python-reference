---
title: "ChnSmooth4253H"
description: "Smoothes a data channel using the 4253H filter."
---

# ChnSmooth4253H

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSmooth4253H

Smoothes a data channel using the 4253H filter.

## Signature

```python
return_value = dd.ChnSmooth4253H( Y , ResultChannel , Smooth4253HTwice )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">Smooth4253HTwice</td>
<td>Specifies whether DIAdem uses the 4253H filter or the 4253H Twice filter. If the value is <span class="Monospace">0</span>, DIAdem uses the 4253H filter. If the value is <span class="Monospace">1</span>, DIAdem uses the 4253H-Twice filter.<div id="exp_Smooth4253HTwice">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= Smooth4253HTwice &lt;= 1<br attr="ext"/>Access: Read/Write</td></tr>
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

*Source: `ComOff/ChnSmooth4253H.htm`*
