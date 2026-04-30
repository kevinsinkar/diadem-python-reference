---
title: "ChnConvertNumericToTime"
description: "Valid names: ChnConvertNumericToTime, ChnNumericToTime"
---

# ChnConvertNumericToTime

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertNumericToTime

Valid names: ChnConvertNumericToTime, ChnNumericToTime

## Signature

```python
return_value = dd.ChnConvertNumericToTime( Y , OffsetStartTime, CreateNewChannel)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the numeric data channel with relative time values, for example, in seconds.</td></tr>
<tr><td width="150">OffsetStartTime</td>
<td>Specifies the start time DIAdem adds as an offset to the numeric values. You create time offsets, for example, with the commands <a href="#" data-unresolved="1">TTR</a> or <a href="../createtime/">CreateTime</a>.<div id="exp_OffsetStartTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CreateNewChannel</td>
<td>Specifies whether DIAdem saves the result in a new channel (TRUE) or whether DIAdem overwrites the input channel with the result (FALSE).<div id="exp_CreateNewChannel">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel as <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a>.</td></tr>
</table>
</div>

## Python example

```python
oMyGroup = dd.Data.Root.ActiveChannelGroup
oMyChannel = oMyGroup.Channels.Add("Numeric", dd.DataTypeChnFloat64)
dd.ChnLinGen(oMyChannel, 1, 100, 100)
oMyDateTime = dd.CreateTime(2018, 12, 11, 12, 13, 14, 123, 0, 0)
oMyResultChn = dd.ChnNumericToTime(oMyChannel, oMyDateTime.VariantDate, True)
oMyResultChn(1).Name = "DateTime"
dd.MsgboxDisp("Result channel: " + oMyGroup.Name + "/" + oMyResultChn(1).Name)
```

```python
MyNumericChn = dd.ChnLinGenImp("Numeric", 100, 1, 1)
MyDateTimeInSecs = dd.TTR("2018-12-11 12:13:14,1230", "#yyyy-mm-dd hh:nn:ss,ffff")
oMyResultChn = dd.ChnNumericToTime(MyNumericChn, MyDateTimeInSecs, True)
oMyResultChn(1).Name = "DateTime"
dd.MsgboxDisp("Result channel: " + oMyResultChn.Item(1).ChannelGroup.Name+ "/"+oMyResultChn.Item(1).Name)
```

---

*Source: `ComOff/ChnConvertNumericToTime.htm`*
