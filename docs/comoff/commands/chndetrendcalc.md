---
title: "ChnDetrendCalc"
description: "Removes a trend in the channel data."
---

# ChnDetrendCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDetrendCalc

Removes a trend in the channel data.

## Signature

```python
return_value = dd.ChnDetrendCalc( XW , Y , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the associated channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the name of the result channel.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel with cleansed values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyGroup = dd.Data.Root.ChannelGroups(1)
oMyTimeChn = oMyGroup.Channels("Time")
oMyDataChn = oMyGroup.Channels("Data")
oMyDetrendChn = oMyGroup.Channels.Add("Detrended", dd.DataTypeChnFloat64)
dd.ChnDetrendCalc(oMyTimeChn, oMyDataChn, oMyDetrendChn)
dd.MsgboxDisp("Result channel: " + oMyGroup.Name + "/" + oMyDetrendChn.Name)
```

```python
oMyResultChn = dd.ChnDetrendCalc("", "[1]/WFData", "/WFDetrended")
dd.MsgboxDisp("Result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnDetrendCalc.htm`*
