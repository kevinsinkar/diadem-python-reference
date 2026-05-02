---
title: "ChnEventCreateFilteredChn"
description: "Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is fulfilled, and otherwise uses"
---

# ChnEventCreateFilteredChn

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCreateFilteredChn

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is fulfilled, and otherwise uses the channel values of a second specified channel.

## Signature

```python
return_value = dd.ChnEventCreateFilteredChn( ResultChannel , ChnEventList , ChnEventFalseChn , ChnEventTrueChn )
```

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
<tr><td width="150">ChnEventTrueChn</td>
<td>Specifies the channel whose values DIAdem copies when the search condition is not fulfilled.<div id="exp_ChnEventTrueChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
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
dd.ChnEventCreateFilteredChn("Event/EventStatusTrueFalse", dd.ChnEventResultList, "[4]/[1]", "[4]/[2]")
```

---

*Source: `ComOff/ChnEventCreateFilteredChn.htm`*
