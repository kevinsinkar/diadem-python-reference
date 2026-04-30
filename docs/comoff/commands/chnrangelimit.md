---
title: "ChnRangeLimit"
description: "Restricts a data channel to the values between an upper and lower limit value. DIAdem replaces the values outside the value range with the upper or lower limit "
---

# ChnRangeLimit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRangeLimit

Restricts a data channel to the values between an upper and lower limit value. DIAdem replaces the values outside the value range with the upper or lower limit value.

## Signature

```python
return_value = dd.ChnRangeLimit( Y , ChnRangeLimitLower, ChnRangeLimitUpper, ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note</strong>  Because DIAdem replaces all curve points outside the range of values with the upper and lower limit value without interpolating the curve at the transitions to the limits, the result curve at the limits shows a different course than the original curve.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the x-values.</td></tr>
<tr><td width="150">ChnRangeLimitLower</td>
<td>Specifies the lower limit to restrict a data channel.<div id="exp_ChnRangeLimitLower">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnRangeLimitUpper</td>
<td>Specifies the upper limit to restrict a data channel.<div id="exp_ChnRangeLimitUpper">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
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
oMyGroup = dd.Data.Root.ActiveChannelGroup
oMyGenSigChn = oMyGroup.Channels.Add("GeneratedSignal", dd.DataTypeChnFloat64)
oMyUppLowChn = oMyGroup.Channels.Add("UpperLowerLimitedChannel", dd.DataTypeChnFloat64)
dd.ChnGenSignal("Sine", 1024, 100, oMyGenSigChn, 3, 2, 0, 0, "s", "V", 50)
dd.ChnRangeLimit(oMyGenSigChn, -1, 1, oMyUppLowChn)
dd.MsgboxDisp("Result channel: " + oMyGroup.Name + "/" + oMyUppLowChn.Name)
```

```python
oMyStartChn = dd.ChnGenSignal("Sine", 1024, 100, "/GeneratedSignal", 3, 2, 0, 0, "s", "V", 50)
oMyResultChn = dd.ChnRangeLimit(oMyStartChn(1), -1, 1, "/UpperLowerLimitedChannel")
dd.MsgboxDisp("Result channel: " + oMyResultChn.Item(1).ChannelGroup.Name+ "/"+oMyResultChn.Item(1).Name)
```

---

*Source: `ComOff/ChnRangeLimit.htm`*
