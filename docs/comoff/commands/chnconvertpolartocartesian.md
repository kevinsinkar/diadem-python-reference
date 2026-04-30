---
title: "ChnConvertPolarToCartesian"
description: "Valid names: ChnConvertPolarToCartesian, ChnPolarToCartesian"
---

# ChnConvertPolarToCartesian

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertPolarToCartesian

Valid names: ChnConvertPolarToCartesian, ChnPolarToCartesian

## Signature

```python
return_value = dd.ChnConvertPolarToCartesian( X , Y , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the angles in radian.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the radii.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that contains the x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that contains the y-values.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels with the Cartesian coordinates. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyGroup = dd.Data.Root.ActiveChannelGroup
oMyAngleChn = dd.Data.GetChannel("[1]/Angle")
oMyRadiusChn = dd.Data.GetChannel("[1]/Radius")
oMyCartesianXChn = oMyGroup.Channels.Add("X-Coordinates", dd.DataTypeChnFloat64)
oMyCartesianYChn = oMyGroup.Channels.Add("Y-Coordinates", dd.DataTypeChnFloat64)
oMyResultChn = dd.ChnPolarToCartesian(oMyAngleChn, oMyRadiusChn, oMyCartesianXChn, oMyCartartesianYChn)
dd.MsgboxDisp("1st Result channel: " + oMyGroup.Name + "/" + oMyCartesianXChn.Name + "\r\n" +"2nd Result channel: " + oMyGroup.Name + "/" + oMyCartesianYChn.Name)
```

```python
oMyResultChn = ChnPolarToComplex("([1]/Angle", "[1]/Radius", "/X-Coordinates", "/Y-Coordinates")
dd.MsgboxDisp("1st Result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name + "\r\n" +"2nd Result channel: " + oMyResultChn(2).ChannelGroup.Name + "/" + oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnConvertPolarToCartesian.htm`*
