---
title: "ChnEventGate"
description: "Connects two search results with the GATE operator. DIAdem interprets the first search result as a list of start events and the second search result as a list o"
---

# ChnEventGate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventGate

Connects two search results with the GATE operator. DIAdem interprets the first search result as a list of start events and the second search result as a list of stop events. The ChnEventGateType setting determines whether DIAdem uses the first or last start event as start and ignores all following start and stop events until the first or the last stop event occurs.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the arrays to be connected do not contain x-values, the third and the fourth column of the result array contains the value <span class="Monospace">Null</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>It only makes sense to concatenate search results if you execute the previous searches in channels that are the same length and contain identical time references to y-values. If you do not meet these conditions, the command does not report errors or issue warnings.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnEventList</td>
<td>Contains the first result of a search or of a logical operation of several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">ChnEventList</td>
<td>Contains the second result of a search or of a logical operation of several searches.<div id="exp_ChnEventList__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">[ChnEventGateType]</td>
<td>Specifies which start event DIAdem uses as start and which stop event as stop. If you do not specify this value, DIAdem uses the setting <span class="Monospace">FirstStartEventFirstStopEvent</span>, which means that DIAdem uses the first start event as start and ignores all following start events until the first stop event occurs. The same applies for multiple stop events. If several stop events occur, DIAdem ignores them until a start event occurs again.<div id="exp_ChnEventGateType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FirstStartEventFirstStopEvent"</pre></donottranslate></td>
<td>First start event with first stop event</td></tr>
<tr><td width="150"><donottranslate><pre>"LastStartEventFirstStopEvent"</pre></donottranslate></td>
<td>Last start event with first stop event</td></tr>
<tr><td width="150"><donottranslate><pre>"FirstStartEventLastStopEvent"</pre></donottranslate></td>
<td>First start event with last stop event</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a two-dimensional array containing the operators of the search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function or define your own variable.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventList1 = None
dd.ChnEventList2 = None
dd.ChnEventResultList = None
dd.ChnEventList1 = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventList2 = dd.ChnEventDetectionWindow("" , "[1]/[3]", 5000, 6500, 0, 0)
dd.ChnEventResultList = dd.ChnEventGATE(dd.ChnEventList1, dd.ChnEventList2)

if dd.Data.GetChannel("[1]/[2]").Size < dd.Data.GetChannel("[1]/[3]").Size :
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
else:
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[3]", 0, 1)
```

---

*Source: `ComOff/ChnEventGate.htm`*
