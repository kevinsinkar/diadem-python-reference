---
title: "ChnConvertTimeToNumeric"
description: "Valid names: ChnConvertTimeToNumeric, ChnTimeToNumeric"
---

# ChnConvertTimeToNumeric

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertTimeToNumeric

Valid names: ChnConvertTimeToNumeric, ChnTimeToNumeric

## Signature

```python
return_value = dd.ChnConvertTimeToNumeric( Y , OffsetCorrection, CreateNewChannel)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the time values.</td></tr>
<tr><td width="150">OffsetCorrection</td>
<td>Determines whether DIAdem subtracts the first time value as offset from the subsequent time values.<div id="exp_OffsetCorrection">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
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
oMyDateTimeInSecs = dd.TTR("2018-12-12 12:12:12,1230", "yyyy-mm-dd hh:nn:ss,ffff")
oMyInputChn = dd.ChnGenTime("DateTime", "second", oMyDateTimeInSecs,None , 1, "StartStepNo", 100)
oMyResultChn = dd.ChnTimeToNumeric(oMyInputChn(1), True, True)
oMyResultChn(1).Name = "Numeric"
dd.MsgboxDisp("Result channel: " + oMyResultChn.Item(1).ChannelGroup.Name + "/" + oMyResultChn.Item(1).Name)
```

---

*Source: `ComOff/ChnConvertTimeToNumeric.htm`*
