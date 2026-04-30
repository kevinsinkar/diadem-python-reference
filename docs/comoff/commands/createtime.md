---
title: "CreateTime"
description: "Creates an object that contains the date and time with a nanoseconds resolution."
---

# CreateTime

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateTime

Creates an object that contains the date and time with a nanoseconds resolution.

## Signature

```python
return_value = dd.CreateTime(iYear, iMonth, iDay, iHour, iMinute, iSecond, [iMillisecond], [iMicrosecond], [iNanosecond])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">iYear</td>
<td>Specifies the year.<div id="exp_iYear">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">iMonth</td>
<td>Specifies the month.<div id="exp_iMonth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">iDay</td>
<td>Specifies the day.<div id="exp_iDay">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">iHour</td>
<td>Specifies the hour.<div id="exp_iHour">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">iMinute</td>
<td>Specifies the minute.<div id="exp_iMinute">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">iSecond</td>
<td>Specifies the second.<div id="exp_iSecond">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[iMillisecond]</td>
<td>Specifies the millisecond.<div id="exp_iMillisecond">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[iMicrosecond]</td>
<td>Specifies the microsecond.<div id="exp_iMicrosecond">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[iNanosecond]</td>
<td>Specifies the nanosecond.<div id="exp_iNanosecond">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../scriptnavi/objects/itdmtimedisp/">UsiTimeDisp object</a> type.</td></tr>
</table>
</div>

## Python example

```python
Range = "week"
oStartTime = dd.CreateTime(1999,11,20,0,0,0)
dStartTime = dd.ConvertTimeType (oStartTime,dd.eConvertDIAdemDateTime )
dd.ChnGenTime ("[]/GenTimeChn_dTime", Range, dStartTime, 0, 1, "StartStepNo", 10)
```

```python
dd.Data.Root.Properties.Add("Time", dd.CreateTime(2004,6,17,10,0,0,0,0,0))
```

---

*Source: `ComOff/CreateTime.htm`*
