---
title: "ChnEventCreateXYChannels"
description: "Specifies whether DIAdem creates a channel with a time channel for each section in which the search condition is met."
---

# ChnEventCreateXYChannels

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCreateXYChannels

Specifies whether DIAdem creates a channel with a time channel for each section in which the search condition is met.

## Signature

```python
return_value = dd.ChnEventCreateXYChannels( XW , Y , ChnEventList , [ChnEventListIndex])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the generated result channels. If you do not specify a time channel, DIAdem does not generate a result time channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the generated result channels.</td></tr>
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
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. The names of the generated channels correspond to the names of the input channels to which the text "-Event" and a number are appended.<br attr="ext"/><a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventList = dd.ChnEventDetectionWindow("", "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventCreateXYChannels("[1]/[1]", "[1]/[2]", dd.ChnEventResultList)
```

---

*Source: `ComOff/ChnEventCreateXYChannels.htm`*
