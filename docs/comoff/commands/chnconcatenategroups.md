---
title: "ChnConcatenateGroups"
description: "Concatenates channels with the same name or the same index of selected groups."
---

# ChnConcatenateGroups

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConcatenateGroups

Concatenates channels with the same name or the same index of selected groups.

## Signature

```python
return_value = dd.ChnConcatenateGroups( ChnConcatenateBaseChannels , ChnConcatenateSourceGroups , ChnConcatenateChannelsByName, ChnConcatenateInPlace, ChnConcatenateMarkBoundaries, ChnConcatenateRestoreWaveform)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnConcatenateBaseChannels</td>
<td>Specifies the channels from the base group to which DIAdem concatenates channels from other groups.<div id="exp_ChnConcatenateBaseChannels">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnConcatenateSourceGroups</td>
<td>Specifies the channel groups containing the channels DIAdem concatenates or adds to the channels of the base group. The order of the channel group specifies the order in which DIAdem concatenates or adds the channels to the base channels. You can only concatenate data channels of the same type.<div id="exp_ChnConcatenateSourceGroups">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">For the <span class="Monospace">ChnConcatenateGroups</span> command, channels with the same names as in the base group or with the same number of channels must be in the channel groups you want to concatenate.</p>
<p class="body">For the <span class="Monospace">ChnConcatenateGroupsAdjustment</span> command, the channel groups can also contain channels that do not exist in the base group. DIAdem supplements the missing group sections in the channels with <span class="Monospace">NoValues</span>.</p>
</div></td></tr>
<tr><td width="150">ChnConcatenateChannelsByName</td>
<td>Specifies that DIAdem concatenates channels with the name (<span class="Monospace">TRUE</span>) or the index (<span class="Monospace">FALSE</span>) of the individual groups.<div id="exp_ChnConcatenateChannelsByName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnConcatenateInPlace</td>
<td>Specifies whether DIAdem overwrites the values of the base channel or channels with results.<div id="exp_ChnConcatenateInPlace">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnConcatenateMarkBoundaries</td>
<td>Specifies that DIAdem inserts a separator after each channel to make the original channels visible. DIAdem inserts <span class="Monospace">NoValue</span> for numeric channels and the following character:<span class="Monospace"> .---.-.</span> for text channels.<div id="exp_ChnConcatenateMarkBoundaries">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnConcatenateRestoreWaveform</td>
<td>Specifies that DIAdem saves the result channels like the input channels as waveform channels if possible. This requires the new time axis of each waveform channel to be continually equidistant.<div id="exp_ChnConcatenateRestoreWaveform">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">If you concatenate waveform channels and the new compound time axis is continually equidistant, DIAdem saves the result in a waveform channel. For example, if the time axes of the individual waveform channels always begin at <span class="Monospace">0 s</span>, DIAdem generates two numeric channels: one with the concatenated time data and one with the measurement data.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels and the result group. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyBaseChannels = dd.Data.CreateElementList()
oMyBaseChannels.Add(dd.Data.Root.ChannelGroups(1).Channels(1))
oMyBaseChannels.Add(dd.Data.Root.ChannelGroups(1).Channels(2))
oMyResultChn = dd.ChnConcatenateGroups(oMyBaseChannels, "'Group2','Group3'", False, False, False, False)
dd.MsgboxDisp("1st Result channel: " + oMyResultChn(1).ChannelGroup.Name+ "/" + oMyResultChn(1).Name + "\r\n" +"2nd Result channel: " + oMyResultChn(2).ChannelGroup.Name+ "/" + oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnConcatenateGroups("'[1]/[1]','[1]/[2]'", "'Group2','Group3'", False, False, False, False)
dd.MsgboxDisp("1st Result channel: " + oMyResultChn(1).ChannelGroup.Name+ "/" + oMyResultChn(1).Name + "\r\n" +"2nd Result channel: " + oMyResultChn(2).ChannelGroup.Name+ "/" + oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnConcatenateGroups.htm`*
