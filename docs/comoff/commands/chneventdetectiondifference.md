---
title: "ChnEventDetectionDifference"
description: "Checks whether two successive single values differ by a certain amount."
---

# ChnEventDetectionDifference

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventDetectionDifference

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Checks whether two successive single values differ by a certain amount.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. You do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnEventDeltaValue</td>
<td>Specifies the sum of the difference value on which DIAdem checks a channel.<div id="exp_ChnEventDeltaValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventDeltaValue &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnEventDeltaType</td>
<td>Specifies the difference type of the difference value on which DIAdem checks a channel.<div id="exp_ChnEventDeltaType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"positive"</pre></donottranslate></td>
<td>Positive</td></tr>
<tr><td width="150"><donottranslate><pre>"negative"</pre></donottranslate></td>
<td>Negative</td></tr>
<tr><td width="150"><donottranslate><pre>"absolute"</pre></donottranslate></td>
<td>Absolute</td></tr>
<tr><td width="150"><donottranslate><pre>"positive-exact"</pre></donottranslate></td>
<td>Positive-exact</td></tr>
<tr><td width="150"><donottranslate><pre>"negative-exact"</pre></donottranslate></td>
<td>Negative-exact</td></tr>
<tr><td width="150"><donottranslate><pre>"absolute-exact"</pre></donottranslate></td>
<td>Absolute-exact</td></tr>
</table>
</td></tr>
</table>
<h2>Valid Settings</h2>
<table class="Borderless">
<tr><td width="150"><donottranslate><pre>"positive"</pre></donottranslate></td>
<td>The difference is positive and greater than or equal to the specified amount.</td></tr>
<tr><td width="150"><donottranslate><pre>"negative"</pre></donottranslate></td>
<td>The difference is negative and greater than or equal to the specified amount.</td></tr>
<tr><td width="150"><donottranslate><pre>"absolute"</pre></donottranslate></td>
<td>The amount of the difference is greater than or equal to the specified amount.</td></tr>
<tr><td width="150"><donottranslate><pre>"positive-exact"</pre></donottranslate></td>
<td>The difference is positive and equal to the specified amount.</td></tr>
<tr><td width="150"><donottranslate><pre>"negative-exact"</pre></donottranslate></td>
<td>The difference is negative and equal to the specified amount.</td></tr>
<tr><td width="150"><donottranslate><pre>"absolute-exact"</pre></donottranslate></td>
<td>The amount of the difference is equal to the specified amount.</td></tr>
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
dd.ChnEventResultList =  dd.ChnEventDetectionDifference("" , "[1]/[3]", 100, "absolute")
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[3]", 0, 1)
```

---

*Source: `ComOff/ChnEventDetectionDifference.htm`*
