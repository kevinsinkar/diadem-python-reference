---
title: "ChnMirror"
description: "Mirrors the data in a channel so that the last channel value comes first."
---

# ChnMirror

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMirror

Mirrors the data in a channel so that the last channel value comes first.

## Signature

```python
return_value = dd.ChnMirror( Y , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values you want to mirror.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the name of the result channel with the mirrored values.</td></tr>
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
oMyGroup = dd.Data.Root.ChannelGroups(1)
oMyChannel = oMyGroup.Channels("Time")
oMyResultChn = oMyGroup.Channels.Add("ChannelMirrored", dd.DataTypeChnDate)
oMyChnResult = dd.ChnMirror(oMyChannel, "[1]/ChannelMirrored")
dd.MsgboxDisp("Result channel: " + oMyGroup.Name + "/" + oMyChnResult(1).Name)
```

```python
oMyResultChn = dd.ChnMirror("[1]/Input", "[1]/ChannelMirrored")
dd.MsgboxDisp("Result channel: " + oMyResultChn.Item(1).ChannelGroup.Name+ "/"+oMyResultChn.Item(1).Name)
```

---

*Source: `ComOff/ChnMirror.htm`*
