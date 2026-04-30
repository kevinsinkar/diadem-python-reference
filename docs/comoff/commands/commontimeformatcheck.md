---
title: "CommonTimeFormatCheck"
description: "Checks whether a time format is commonly applicable and specifies a universal format string."
---

# CommonTimeFormatCheck

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CommonTimeFormatCheck

Checks whether a time format is commonly applicable and specifies a universal format string.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>A commonly applicable time format in DIAdem contains the complete format specifications for day (<span class="Monospace">dd</span>) and month (<span class="Monospace">mm</span>), and a four figure year specification (<span class="Monospace">yyyy</span>). You can use dashes (-), dots (.), and slashes (/) as separators, in commonly applicable time formats. Use format specifications that are separated with a colon for hours, minutes, and seconds. For example <span class="Monospace">#dd.mm.yyyy hh:nn:ss</span>, <span class="Monospace">#yyyy/mm/dd hh:nn:ss</span>, or <span class="Monospace">#mm/dd/yyyy hh:nn:ss</span> are universal.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CommonTimeFormat</td>
<td>Specifies the format string to be checked. Receives a universal time format after the <a href="./">CommonTimeFormatCheck</a> command is called.<div id="exp_CommonTimeFormat">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean</a> type. If the time format to be checked is commonly applicable, the command returns <span class="Monospace">TRUE</span>, otherwise <span class="Monospace">FALSE</span>. The variable <a href="../../../varoff/variables/commontimeformat/">CommonTimeFormat</a> contains an appropriate universal time format.</td></tr>
</table>
</div>

## Python example

```python
import datetime
MyFormat ="#mm/dd/yy hh:nn"
bIsCommon = dd.CommonTimeFormatcheck(MyFormat)
#TimeFormat = CommonTimeFormat
if not bIsCommon :
    dd.MsgBoxDisp ("Your time format:" + "\r\n" + dd.Str(datetime.datetime.now(), MyFormat) + "\r\n" + "This was changes to the common time format:" + "\r\n" + dd.Str(datetime.datetime.now(), dd.CommonTimeFormat))
```

---

*Source: `ComOff/CommonTimeFormatCheck.htm`*
