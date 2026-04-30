---
title: "ChnEventDuration"
description: "Specifies the duration of individual events or of all events from the results list of an event search."
---

# ChnEventDuration

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventDuration

Specifies the duration of individual events or of all events from the results list of an event search.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong>This command only leads to meaningful results if you use the time reference of the values to be checked in the previous event search. Therefore specify a waveform channel as the y-channel in the event search or specify explicitly an x-channel for the search.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnEventList</td>
<td>Contains the search result or the result of a logical operation from several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">[ChnEventListIndex]</td>
<td>Specifies the index of the event. If the index is not specified or if <span class="Monospace">Null</span> is specified, DIAdem includes all events.<div id="exp_ChnEventListIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventList1 = dd.ChnEventDetectionWindow("[1]/[1]", "[1]/[3]", 5000, 6100, 0, 0)
if dd.ChnEventCount(dd.ChnEventList1) > 0 :
    dResult = dd.ChnEventDuration(dd.ChnEventList1, 1)
    print("Duration of first event: " + dResult)
```

---

*Source: `ComOff/ChnEventDuration.htm`*
