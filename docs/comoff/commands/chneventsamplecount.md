---
title: "ChnEventSampleCount"
description: "Specifies the number of values of an individual event or of all events from the results list of an event search. Use the ChnEventStatValueCount command to count"
---

# ChnEventSampleCount

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventSampleCount

Specifies the number of values of an individual event or of all events from the results list of an event search. Use the ChnEventStatValueCount command to count only those values at which the specified channel does not contain any NoValues.

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
<td>The return value is a <a href="#" data-unresolved="1">Longinteger</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
sOutPut = "Statistic results for events:" + "\r\n" + "Number of values: "
for iCount in range( 1, dd.ChnEventCount(dd.ChnEventResultList)+1):
    sOutPut = sOutPut + " Event " + iCount + ": " + dd.ChnEventSampleCount(dd.ChnEventResultList, iCount)
print(sOutPut)
```

---

*Source: `ComOff/ChnEventSampleCount.htm`*
