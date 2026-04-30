---
title: "ChnDiv"
description: "Divides two channels."
---

# ChnDiv

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDiv

Divides two channels.

## Signature

```python
return_value = dd.ChnDiv( Y , Y1 , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the dividend values.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the divisor values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
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
MyResultChn = dd.ChnDiv("Group1/Channel1","Group1/Channel2","Divided")
```

---

*Source: `ComOff/ChnDiv.htm`*
