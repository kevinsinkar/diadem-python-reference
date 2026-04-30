---
title: "ChnPhaseWrap"
description: "Wraps phases in a channel."
---

# ChnPhaseWrap

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPhaseWrap

Wraps phases in a channel.

## Signature

```python
return_value = dd.ChnPhaseWrap( Y , ResultChannel , PhaseWrapBegin, PhaseWrapEnd)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">PhaseWrapBegin</td>
<td>Specifies the smallest value of the input channel.<div id="exp_PhaseWrapBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PhaseWrapEnd</td>
<td>Specifies the greatest value of the input channel.<div id="exp_PhaseWrapEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
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
import math
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyResultChn = dd.ChnPhaseWrap(oMyYChannel, "Results/PhaseWrapped", - math.pi, math.pi)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
import math
oMyResultChn = dd.ChnPhaseWrap("[1]/[1]","Results/PhaseWrapped", - math.pi, math.pi)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnPhaseWrap.htm`*
