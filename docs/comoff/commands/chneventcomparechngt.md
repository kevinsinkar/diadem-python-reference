---
title: "ChnEventCompareChnGT"
description: "Determines the area in a data channel in which the value is greater than the value of the second channel."
---

# ChnEventCompareChnGT

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventCompareChnGT

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Determines the area in a data channel in which the value is greater than the value of the second channel.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the xw-values of the first channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the first channel.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the y-values of the second channel.</td></tr>
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
dd.ChnEventResultList= None
dd.ChnEventResultList =  dd.ChnEventCompareChnGT("" , "[1]/[2]", "[1]/[3]")
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

---

*Source: `ComOff/ChnEventCompareChnGT.htm`*
