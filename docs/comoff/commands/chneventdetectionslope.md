---
title: "ChnEventDetectionSlope"
description: "Checks whether the values of a channel exceed a limit value in the specified slope direction. You can search for rising and falling slopes and specify an option"
---

# ChnEventDetectionSlope

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventDetectionSlope

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

Checks whether the values of a channel exceed a limit value in the specified slope direction. You can search for rising and falling slopes and specify an optional hysteresis range.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the xw-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnEventSlopeLevel</td>
<td>Specifies the value that must be exceeded or undershot before DIAdem checks the slope direction.<div id="exp_ChnEventSlopeLevel">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventSlopeType</td>
<td>Specifies the slope direction.<div id="exp_ChnEventSlopeType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"increasing"</pre></donottranslate></td>
<td>Increasing</td></tr>
<tr><td width="150"><donottranslate><pre>"decreasing"</pre></donottranslate></td>
<td>Decreasing</td></tr>
<tr><td width="150"><donottranslate><pre>"both"</pre></donottranslate></td>
<td>Rising and falling</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnEventSlopeLevelHysteresis]</td>
<td>Specifies the hysteresis value for the slope value. If the search searches for rising slopes, the hysteresis window is below the slope value. If the search searches for falling slopes, the hysteresis is above the slope value. If the search searches for rising and falling slopes, DIAdem uses two hysteresis windows. The default value is <span class="Monospace">0</span> and means that DIAdem does not use a hysteresis.<div id="exp_ChnEventSlopeLevelHysteresis">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventSlopeLevelHysteresis &lt;= 1E300</td></tr>
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
<td>Specifies the maximum number of result values. The default value is <span class="Monospace">0</span> and means that DIAdem does not use all result values.<div id="exp_ChnEventMaxResultCount">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventMaxResultCount &lt;= 2147483647</td></tr>
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
dd.ChnEventResultList = None
dd.ChnEventResultList =  dd.ChnEventDetectionSlope("" , "[1]/[2]", 40, "both", 0)
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

```python
dd.ChnEventList1 = None
dd.ChnEventList2 = None
dd.ChnEventResultList = None
dd.ChnEventList1 = dd.ChnEventDetectionSlope("" , "[1]/[2]", 40, "both", 0)
dd.ChnEventList2 = dd.ChnEventDetectionWindow("" , "[1]/[3]", 5500, 6500, 0, 0)
dd.ChnEventResultList = dd.ChnEventOperationAND(dd.ChnEventList1, dd.ChnEventList2)

if dd.Data.GetChannel("[1]/[2]").Size < dd.Data.GetChannel("[1]/[3]").Size :
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
else:
    dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[3]", 0, 1)
```

---

*Source: `ComOff/ChnEventDetectionSlope.htm`*
