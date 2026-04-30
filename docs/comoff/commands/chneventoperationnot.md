---
title: "ChnEventOperationNOT"
description: "Negates a search result with the NOT operator. The length of channel SourceChn specifies the maximum index of the result array."
---

# ChnEventOperationNOT

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventOperationNOT

Negates a search result with the NOT operator. The length of channel SourceChn specifies the maximum index of the result array.

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
<tr><td width="150">SourceChn</td>
<td>Specifies the input channel.<div id="exp_SourceChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to specify channels.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a two-dimensional array containing the operators of the search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function, or define your own variable.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
dd.ChnEventResultList = dd.ChnEventOperationNOT(dd.ChnEventResultList,"[1]/[2]")
dd.ChnEventCreateStatusChn("Event/EventStatusNOT", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

---

*Source: `ComOff/ChnEventOperationNOT.htm`*
