---
title: "ChnEventDetectionWindow"
description: "Checks whether the values of a channel are in a specified window. You can specify an optional hysteresis range for the upper and lower window limit."
---

# ChnEventDetectionWindow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventDetectionWindow

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

Checks whether the values of a channel are in a specified window. You can specify an optional hysteresis range for the upper and lower window limit.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the xw-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnEventWindowLowerLimit</td>
<td>Specifies the lower limit value for which DIAdem checks the channel. If the value is <span class="Monospace">NOVALUE</span>, DIAdem uses a value range without a lower limit.<div id="exp_ChnEventWindowLowerLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventWindowUpperLimit</td>
<td>Specifies the top limit value for which DIAdem checks the channel. If the value is <span class="Monospace">NOVALUE</span>, DIAdem uses a value range without an upper limit.<div id="exp_ChnEventWindowUpperLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventWindowLowerLimitHysteresis]</td>
<td>Specifies the value of the hysteresis for the bottom limit value of the value range. DIAdem positions a hysteresis window, which is twice as wide as the specified value, centric around the bottom limit value. The default value is <span class="Monospace">0</span> and means that DIAdem does not use a hysteresis.<div id="exp_ChnEventWindowLowerLimitHysteresis">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventWindowLowerLimitHysteresis &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventWindowUpperLimitHysteresis]</td>
<td>Specifies the value of the hysteresis for the top limit value of the value range. DIAdem positions a hysteresis window, which is twice as wide as the specified value, centric around the top limit value. The default value is <span class="Monospace">0</span> and means that DIAdem does not use a hysteresis.<div id="exp_ChnEventWindowUpperLimitHysteresis">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventWindowUpperLimitHysteresis &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventBeginIndex]</td>
<td>Specifies at which line number DIAdem starts checking the values of the data channel. The default value is <span class="Monospace">0</span>, which means that DIAdem starts checking the values from the first row.<div id="exp_ChnEventBeginIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventBeginIndex &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventEndIndex]</td>
<td>Specifies the line number up to which DIAdem checks the values of the data channel. The default value is <span class="Monospace">0</span>, which means that DIAdem checks the values up to the last row.<div id="exp_ChnEventEndIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventEndIndex &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventMaxResultCount]</td>
<td>Specifies the maximum number of result values. The default value is <span class="Monospace">0</span> and means that DIAdem uses all result values.<div id="exp_ChnEventMaxResultCount">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventMaxResultCount &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventCloseOnNoValue]</td>
<td>Specifies whether DIAdem uses a <span class="Monospace">NoValue</span> at the end of the value area searched for. The default value is <span class="Monospace">FALSE</span>, which means that DIAdem ignores <span class="Monospace">NoValues</span>.<div id="exp_ChnEventCloseOnNoValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventUseFirstXValueOutside]</td>
<td>Specifies whether DIAdem uses the last x-value that meets the condition as the end of the wanted value range or the next value. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem uses the last x-value as the end of the wanted value range. The <span class="Monospace">ChnEventUseFirstXValueOutside</span> only influences the x-value index but not the value index.<div id="exp_ChnEventUseFirstXValueOutside">
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
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>A return value is a two-dimensional array containing the search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function, or define your own variable.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnEventResultList= None
dd.ChnEventResultList = dd.ChnEventDetectionWindow("" , "[1]/[2]", 40, 50, 0, 0)
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

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

*Source: `ComOff/ChnEventDetectionWindow.htm`*
