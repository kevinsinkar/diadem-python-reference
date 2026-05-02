---
title: "ChnEventFind"
description: "Determines the area in a data channel that meets a specified condition."
---

# ChnEventFind

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventFind

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('ChnEventResultList', ...)   # instead of dd.ChnEventResultList = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Determines the area in a data channel that meets a specified condition.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note </strong>When comparing two channels in the formula, DIAdem uses the functions <a href="../chneventcomparechneq/">ChnEventCompareChnEQ</a>, <a href="../chneventcomparechnge/">ChnEventCompareChnGE</a>, <a href="../chneventcomparechngt/">ChnEventCompareChnGT</a>, <a href="../chneventcomparechnle/">ChnEventCompareChnLE</a>, <a href="../chneventcomparechnlt/">ChnEventCompareChnLT</a>, and <a href="../chneventcomparechnne/">ChnEventCompareChnNE</a> if possible.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CalculateFormula</td>
<td>Specifies a formula in a script. Enter the formula in quotation marks. You must enclose texts that are in quotation marks, such as channel names, in double quotation marks.<div id="exp_CalculateFormula">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">CalculateSymbols</td>
<td>Specifies a list with symbol names, which are replaced in the formula with values. The symbols <span class="Monospace">CalculateSymbols</span> and the values <span class="Monospace">CalculateValues</span> are assigned through their field index.<div id="exp_CalculateSymbols">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">CalculateValues</td>
<td>Specifies a list of the values associated with the symbols. The symbols <span class="Monospace">CalculateSymbols</span> and the values <span class="Monospace">CalculateValues</span> are assigned through their field index.<div id="exp_CalculateValues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p>The <span class="Monospace">CalculateValues</span> vector can contain numeric values, texts, <a href="../../../ivalueunit/objects/ivalueunit/">Value-Unit objects</a>, and <a href="../../../inavidata/objects/idiademchannel/">Channel objects</a>. DIAdem interprets the value-unit objects like the <a href="#" data-unresolved="1">VU</a> function and channel objects like the <a href="../../../varoff/variables/ch/">Ch</a> variable.</p>
</div></td></tr>
<tr><td width="150">[ChnEventHysteresis]</td>
<td>Specifies the hysteresis value for the check value. DIAdem interprets this value as a percentage of the value to check. The default value is <span class="Monospace">0</span> and means that DIAdem does not use a hysteresis.<div id="exp_ChnEventHysteresis">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ChnEventHysteresis &lt;= 100</td></tr>
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
dd.ChnEventResultList = None
dd.ChnEventResultList = dd.ChnEventFind("(A>40) and (B>200)", ["A","B"], [dd.Data.GetChannel("[1]/[2]"),dd.Data.GetChannel("[1]/[3]")])
dd.ChnEventCreateStatusChn("Event/EventStatus", dd.ChnEventResultList, "[1]/[2]", 0, 1)
```

---

*Source: `ComOff/ChnEventFind.htm`*
