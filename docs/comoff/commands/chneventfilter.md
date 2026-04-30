---
title: "ChnEventFilter"
description: "Checks whether a search result contains short phases in which an event is fulfilled or not fulfilled, and filters these positive or negative peaks from the sear"
---

# ChnEventFilter

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventFilter

Checks whether a search result contains short phases in which an event is fulfilled or not fulfilled, and filters these positive or negative peaks from the search results.

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
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">ChnEventFilterType</td>
<td>Specifies to which events the filter should apply. In the case of <span class="Monospace">"Peaks"</span>, the filter applies to fulfilled events, in the case of <span class="Monospace">"Valleys"</span> it applies to unfulfilled events.<div id="exp_ChnEventFilterType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Peaks"</pre></donottranslate></td>
<td>Peaks</td></tr>
<tr><td width="150"><donottranslate><pre>"Valleys"</pre></donottranslate></td>
<td>Valleys</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventFilterValue</td>
<td>Specifies the width of the filter.<div id="exp_ChnEventFilterValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventFilterValue &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventFilterValueType</td>
<td>Specifies whether the function interprets the value of the variable <span class="Monospace">ChnEventFilterValue</span> as index or as x-value.<div id="exp_ChnEventFilterValueType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Index"</pre></donottranslate></td>
<td>Index</td></tr>
<tr><td width="150"><donottranslate><pre>"Value"</pre></donottranslate></td>
<td>Value</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>A return value is a two-dimensional array containing the search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function or define your own variable.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventList1 = None
dd.ChnEventList2 = None
dd.ChnEventList1 = dd.ChnEventDetectionDifference("" , "[1]/[3]", 100, "absolute")
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventList1, "[1]/[2]", 0, 1)

dd.ChnEventList2 = dd.ChnEventFilter(dd.ChnEventList1, "Peaks", 5 , "Index")
dd.ChnEventCreateStatusChn("Event/EventStatusFiltered", dd.ChnEventList2, "[1]/[2]", 0, 1)
```

---

*Source: `ComOff/ChnEventFilter.htm`*
