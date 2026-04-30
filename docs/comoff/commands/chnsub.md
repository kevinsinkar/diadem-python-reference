---
title: "ChnSub"
description: "Subtracts one channel from another."
---

# ChnSub

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSub

Subtracts one channel from another.

## Signature

```python
return_value = dd.ChnSub( Y , Y1 , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing minuend values.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the subtrahend values.</td></tr>
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
MyResultChn = dd.ChnSub("Group1/Channel1","Group1/Channel2")
```

---

*Source: `ComOff/ChnSub.htm`*
