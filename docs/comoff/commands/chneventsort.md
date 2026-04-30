---
title: "ChnEventSort"
description: "Sorts the results list of an event search according to its length."
---

# ChnEventSort

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventSort

Sorts the results list of an event search according to its length.

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
<tr><td width="150">ChnEventSortType</td>
<td>Specifies the sorting direction.<div id="exp_ChnEventSortType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"upward"</pre></donottranslate></td>
<td>Ascending</td></tr>
<tr><td width="150"><donottranslate><pre>"downward"</pre></donottranslate></td>
<td>Descending</td></tr>
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
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
sOutPut = "Without sorting: "
for iCount in range( 1, dd.ChnEventCount(dd.ChnEventResultList)+1):
    sOutPut = sOutPut + " Event " + iCount + ": " + dd.ChnEventSampleCount(dd.ChnEventResultList, iCount)
dd.ChnEventResultList = dd.ChnEventSort(dd.ChnEventResultList, "upward")
sOutPut = sOutPut + "\r\n" + "After sorting: "
for iCount in range( 1, dd.ChnEventCount(dd.ChnEventResultList)+1):
    sOutPut = sOutPut + " Event " + iCount + ": " + dd.ChnEventSampleCount(dd.ChnEventResultList, iCount)
print(sOutPut)
```

---

*Source: `ComOff/ChnEventSort.htm`*
