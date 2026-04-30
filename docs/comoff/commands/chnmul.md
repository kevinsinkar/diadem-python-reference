---
title: "ChnMul"
description: "Multiplies two or more channels."
---

# ChnMul

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMul

Multiplies two or more channels.

## Signature

```python
return_value = dd.ChnMul( Y , CALCYChn, ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with the values you want to multiply.</td></tr>
<tr><td width="150">CALCYChn</td>
<td>Specifies the data channels containing the y-values of the signal.<div id="exp_CALCYChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
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
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
MyMultipleResultChn = dd.ChnMul("Group1/Channel1", oMyChannelList, "[1]/Multiplied")
```

---

*Source: `ComOff/ChnMul.htm`*
