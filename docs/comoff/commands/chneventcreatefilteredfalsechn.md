---
title: "ChnEventCreateFilteredFalseChn"
description: "Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is not fulfilled, and otherwise "
---

# ChnEventCreateFilteredFalseChn

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCreateFilteredFalseChn

Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is not fulfilled, and otherwise uses a specified value.

## Signature

```python
return_value = dd.ChnEventCreateFilteredFalseChn( ResultChannel , ChnEventList , ChnEventFalseChn , ChnEventTrueValue )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the transferred channel is a waveform channel, the result channel adopts the waveform properties.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">ChnEventList</td>
<td>Contains the result of a search or the result of the logical operation of several searches.<div id="exp_ChnEventList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">This variable corresponds with a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">ChnEventFalseChn</td>
<td>Specifies the channel whose values DIAdem copies when the search condition is not fulfilled.<div id="exp_ChnEventFalseChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventTrueValue</td>
<td>Specifies the value which DIAdem stores in the result channel when the search is fulfilled. The default value is <span class="Monospace">1</span>.<div id="exp_ChnEventTrueValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
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
dd.ChnEventResultList = None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[4]/[1]", 28, 32, 0, 0)
dd.ChnEventCreateFilteredFalseChn ("Event/EventStatusFalse", dd.ChnEventResultList, "[4]/[1]", 1)
```

---

*Source: `ComOff/ChnEventCreateFilteredFalseChn.htm`*
