---
title: "MatChnConvert"
description: "Converts three-dimensional data matrices, including the x and the y-channel, into a data triplet."
---

# MatChnConvert

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatChnConvert

Converts three-dimensional data matrices, including the x and the y-channel, into a data triplet.

## Signature

```python
return_value = dd.MatChnConvert( X , Y , ChnList, ResultChannel , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
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
<td>Specifies the result channel for the x-values of the data triplet.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the y-values of the data triplet.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the z-values of the data triplet.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains three result channels with the x-, y- and z-values of data triplet. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/*")
oMyResultChn = dd.MatChnConvert(oMyXChannel, oMyYChannel, oMyChannelList, "Results/ConvertedTripleX", "Results/ConvertedTripleY", "Results/ConvertedTripleZ")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatChnConvert("[2]/[1]", "[2]/[2]", oMyChannelList, "Results/ConvertedTripleX", "Results/ConvertedTripleY", "Results/ConvertedTripleZ")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

---

*Source: `ComOff/MatChnConvert.htm`*
