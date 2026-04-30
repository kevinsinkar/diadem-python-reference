---
title: "ChnEventCopyValues"
description: "Copies the values of an event search into new channels."
---

# ChnEventCopyValues

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCopyValues

Copies the values of an event search into new channels.

## Signature

```python
return_value = dd.ChnEventCopyValues( XW , Y , ResultChannel , ResultChannel , ChnEventList , [ChnEventListIndex], [ ChnEventSetSeparator ])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the associated y-channel is waveform or xy-channel or you only want to copy y-values, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel of the x-channel. DIAdem generates the x-channel, even if a data channel containing the xw-channel was specified. DIAdem also generates the x-channel if the y-channel is a waveform channel and DIAdem finds several events and copies them into a result channel.<br attr="ext"/>If DIAdem copies several events to an event channel, DIAdem separates the results with a NoValue.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel of the y-channel.<br attr="ext"/>If DIAdem copies several events to an event channel, DIAdem separates the results with a NoValue.</td></tr>
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
<tr><td width="150">[ChnEventSetSeparator]</td>
<td>Specifies whether DIAdem separates event areas with a NoValue.<div id="exp_ChnEventSetSeparator">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
if not dd.ChnEventResultList == None :
    dd.ChnEventCopyValues("" ,"[1]/[2]", "Event/EventresultX", "Event/EventresultY", dd.ChnEventResultList)
```

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 0.40, 0.50, 0, 0)
if not dd.ChnEventResultList == None :
    for iCount in range( 1, dd.ChnEventCount(dd.ChnEventResultList)+1):
        dd.ChnEventCopyValues("" , "[1]/[2]", "Event/EventresultX", "Event/EventresultY" + iCount, dd.ChnEventResultList, iCount)
```

---

*Source: `ComOff/ChnEventCopyValues.htm`*
