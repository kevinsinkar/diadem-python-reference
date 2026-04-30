---
title: "ChnConvertCartesianToPolar"
description: "Valid names: ChnConvertCartesianToPolar, ChnCartesianToPolar"
---

# ChnConvertCartesianToPolar

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertCartesianToPolar

Valid names: ChnConvertCartesianToPolar, ChnCartesianToPolar

## Signature

```python
return_value = dd.ChnConvertCartesianToPolar( X , Y , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the angles in radian.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the radii.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels with the polar coordinates. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyGroup = dd.Data.Root.ActiveChannelGroup
oMyCartesianXChn = dd.Data.GetChannel("[1]/XCartesian")
oMyCartesianYChn = dd.Data.GetChannel("[1]/YCartesian")
oMyAngleChn = oMyGroup.Channels.Add("PolarAngle", dd.DataTypeChnFloat64)
oMyRadiusChn = oMyGroup.Channels.Add("PolarRadius", dd.DataTypeChnFloat64)
oMyResultChn = dd.ChnCartesianToPolar(oMyCartesianXChn, oMyCartesianYChn, oMyAngleChn, oMyRadiusChn)
dd.MsgboxDisp("1st Result channel: " + oMyGroup.Name + "/" + oMyPhasChn.Name + "\r\n" +"2nd Result channel: " + oMyGroup.Name + "/" + oMyAmplChn.Name)
```

```python
oMyResultChn = dd.ChnCartesianToPolar("[1]/XCartesian", "[1]/YCartesian", "/PolarAngle", "/PolarRadius")
dd.MsgboxDisp("1st Result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name + "\r\n" +"2nd Result channel: " + oMyResultChn(2).ChannelGroup.Name + "/" + oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnConvertCartesianToPolar.htm`*
