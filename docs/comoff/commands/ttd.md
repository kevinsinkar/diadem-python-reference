---
title: "TTD"
description: "Converts a text from a time format to a VBS date: A VBS date is a Variant type with the subtype Date . VBS processes data in the range of 01/01/100 to 31/12/999"
---

# TTD

!!! abstract "Command &middot; `ComOff.chm`"
    Command: TTD

Converts a text from a time format to a VBS date: A VBS date is a Variant type with the subtype Date . VBS processes data in the range of 01/01/100 to 31/12/9999 23:59:59 .

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DateTimeString</td>
<td>Specifies a text or a variable that contains the date in DIAdem time format. The text must not contain written or abbreviated weekdays, months, or calendar weeks. If the day or month is single-digit, it must contain leading zeros, for example, <span class="Monospace">01/01/2015</span>.<div id="exp_DateTimeString">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[DateTimeFormat]</td>
<td>Specifies the time format for the text according to the <a href="#" data-unresolved="1">format instructions</a>. If you do not specify a time format, DIAdem applies the default format specified under <strong>Settings»DIAdem Settings</strong>.<div id="exp_DateTimeFormat">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Return value VBS date which is a <a href="#" data-unresolved="1">Variant</a> type with the subtype <span class="Monospace">Date</span>.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
strMyResult = FileDateGet(LayoutLibrPath + "Example.tdr","fdModify")
MyDate = TTD(strMyResult)
MsgBoxDisp(WeekDayName(Weekday(MyDate)))
```

---

*Source: `ComOff/TTD.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
