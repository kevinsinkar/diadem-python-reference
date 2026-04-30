---
title: "ChnWfPropSet"
description: "Sets the waveform property of channels. If the specified channels are not waveform channels, DIAdem converts the channels into waveform channels. When you conve"
---

# ChnWfPropSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnWfPropSet

Sets the waveform property of channels. If the specified channels are not waveform channels, DIAdem converts the channels into waveform channels. When you convert an xy-channel to a waveform channel, DIAdem automatically removes the xy relationship.

## Signature

```python
dd.ChnWfPropSet(ChnList, WfXName, WfXUnitString, WfStartOffset, WfIncrement, [WfStartTime])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you enter as a start time a value prior to 01/01/1600 01:00:00 AM or after 12/31/3000 11:59:59 PM, LabVIEW ignores this start time.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">WfXName</td>
<td>Specifies the name of the x-part of the waveform channel.<div id="exp_WfXName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">WfXUnitString</td>
<td>Specifies the unit of the x-part of the waveform channel.<div id="exp_WfXUnitString">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">WfStartOffset</td>
<td>Specifies the offset of the x-part of the waveform channel.<div id="exp_WfStartOffset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">WfIncrement</td>
<td>Specifies the step width of the x-part of the waveform channel.<div id="exp_WfIncrement">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[WfStartTime]</td>
<td>Specifies the start time of the x-part of the waveform channel. The default value is <span class="Monospace">01/01/1904 00:00:00</span><div id="exp_WfStartTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p>Value range: 01/01/0000 00:00:00 &lt;= WfStartTime &lt;= 12/31/9999 23:59:59</p>
<p>You can transfer double type values and date/time type values to the <span class="Monospace">WfStartTime</span> parameter.</p>
<p></p><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you enter as a start time a value prior to 01/01/1600 01:00:00 AM or after 12/31/3000 11:59:59 PM, LabVIEW ignores this start time.</td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
import datetime
#Value of date/time type
sVal = dd.RTT(datetime.datetime.now())
dd.ChnWfPropSet("[1]/Channel", "Time", "s" , 1, 0.01, sVal)
```

---

*Source: `ComOff/ChnWfPropSet.htm`*
