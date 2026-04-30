---
title: "ChnPhaseUnwrap"
description: "Unwraps phases in a channel."
---

# ChnPhaseUnwrap

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPhaseUnwrap

Unwraps phases in a channel.

## Signature

```python
return_value = dd.ChnPhaseUnwrap( Y , ResultChannel , PhaseUnwrapBegin, PhaseUnwrapEnd)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">PhaseUnwrapBegin</td>
<td>Specifies the smallest value of the input channel.<div id="exp_PhaseUnwrapBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PhaseUnwrapEnd</td>
<td>Specifies the greatest value of the input channel.<div id="exp_PhaseUnwrapEnd">
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
oMyResultChn = dd.ChnPhaseUnwrap(oMyYChannel, "Results/PhaseUnwrapped", - math.pi, math.pi)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
import math
oMyResultChn = dd.ChnPhaseUnwrap("[1]/[1]", "Results/PhaseUnwrapped", - math.pi, math.pi)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnPhaseUnwrap.htm`*
