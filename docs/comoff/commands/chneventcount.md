---
title: "ChnEventCount"
description: "Specifies the number of results in an event search."
---

# ChnEventCount

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCount

Specifies the number of results in an event search.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnEventList</td>
<td>Contains the result of a search or the result of the logical operation of several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds with a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Integer</a> type.</td></tr>
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

*Source: `ComOff/ChnEventCount.htm`*
