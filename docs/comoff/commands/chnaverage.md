---
title: "ChnAverage"
description: "Calculates the arithmetic means of the single values of several data channels."
---

# ChnAverage

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnAverage

Calculates the arithmetic means of the single values of several data channels.

## Signature

```python
return_value = dd.ChnAverage(ChnList, ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
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
dd.ChnAverage(oMyChannelList, "[1]/Average")
```

---

*Source: `ComOff/ChnAverage.htm`*
