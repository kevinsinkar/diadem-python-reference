---
title: "ChnEventCreateStatusChn"
description: "Creates a result channel from the search results."
---

# ChnEventCreateStatusChn

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCreateStatusChn

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    bridge.TextVarSet('ChnEventList1', ...)   # instead of dd.ChnEventList1 = ...
    bridge.TextVarSet('ChnEventList2', ...)   # instead of dd.ChnEventList2 = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Creates a result channel from the search results.

## Signature

```python
return_value = dd.ChnEventCreateStatusChn( ResultChannel , ChnEventList , ChnEventChnArg , [ ChnEventFalseValue ], [ ChnEventTrueValue ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The structure of the result channel enables you to use this channel, for example, to display a background segment in DIAdem VIEW or DIAdem REPORT.</td></tr></table>
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
<p class="body">This variable corresponds to a two-dimensional array which can receive a search result or its operator. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array.</p>
</div></td></tr>
<tr><td width="150">ChnEventChnArg</td>
<td>Specifies the channel whose length specifies the maximum number of values of the result channel. If the specified channel is a waveform channel, DIAdem also transfers the waveform properties to the result channel.<div id="exp_ChnEventChnArg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventFalseValue]</td>
<td>Specifies the value which DIAdem stores in the result channel when the search is not fulfilled. The default value is <span class="Monospace">0</span>.<div id="exp_ChnEventFalseValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventTrueValue]</td>
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
dd.ChnEventList1 = None
dd.ChnEventList2 = None
dd.ChnEventResultList = None
dd.ChnEventList1 = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventList2 = dd.ChnEventDetectionWindow("" , "[1]/[3]", 5500, 6500, 0, 0)
dd.ChnEventResultList = dd.ChnEventOperationAND(dd.ChnEventList1, dd.ChnEventList2)

if dd.Data.GetChannel("[1]/[2]").Size < dd.Data.GetChannel("[1]/[3]").Size :
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
else:
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[3]", 0, 1)
```

---

*Source: `ComOff/ChnEventCreateStatusChn.htm`*
