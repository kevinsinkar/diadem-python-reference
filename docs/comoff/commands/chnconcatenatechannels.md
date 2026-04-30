---
title: "ChnConcatenateChannels"
description: "Concatenates individual channels"
---

# ChnConcatenateChannels

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConcatenateChannels

Concatenates individual channels

## Signature

```python
return_value = dd.ChnConcatenateChannels( Y , ChnConcatenateSourceChannels , ChnConcatenateInPlace, ChnConcatenateMarkBoundaries, ChnConcatenateRestoreWaveform)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the base channel to which DIAdem concatenates further channels.</td></tr>
<tr><td width="150">ChnConcatenateSourceChannels</td>
<td>Specifies the channels which DIAdem concatenates to the base channel. The order of the channels specifies the order in which DIAdem concatenates these channels to the base channel. You can only concatenate data channels of the same type.<div id="exp_ChnConcatenateSourceChannels">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
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
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyConcatChns = dd.Data.GetChannels("Data*") # "Data1", Data2", "Data3", ...
oMyBaseChn = oMyConcatChns(1)
oMyConcatChns.Remove(1)
oMyResultChn = dd.ChnConcatenateChannels(oMyBaseChn, oMyConcatChns, True, False, False)
oMyResultChn(1).Name = "Data All"
dd.MsgboxDisp("Result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name)
```

```python
oMyResultChn = dd.ChnConcatenateChannels("Data1", "'Data2','Data3'", False, False, False)
oMyResultChn(1).Name = "Data All"
dd.MsgboxDisp("Result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnConcatenateChannels.htm`*
