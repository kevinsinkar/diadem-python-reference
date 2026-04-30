---
title: "ChnGenTime"
description: "Generates a time channel with equidistant values."
---

# ChnGenTime

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGenTime

Generates a time channel with equidistant values.

## Signature

```python
return_value = dd.ChnGenTime( ResultChannel , GenTimeUnit, GenTimeXBeg, GenTimeXEnd, GenTimeStep, GenTimeMode, GenTimeNo)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you specify a time unit of microseconds, the time format, for example, <span class="Monospace">#dd.mm.yyyy hh:nn:ss.ffff</span> can display a minimum of 100 microsecond steps.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you select the selection term <span class="Monospace">“StartStepEnd”</span> for the <span class="Monospace">GenTimeMode</span>, the command uses the input parameters <span class="Monospace">GenTimeXBeg</span>, <span class="Monospace">GenTimeStep</span>, and <span class="Monospace">GenTimeXEnd</span>. If you select <span class="Monospace">“StartStepNo”</span> for <span class="Monospace">GenTimeMode</span>, the command uses the input parameters <span class="Monospace">GenTimeXBeg</span>, <span class="Monospace">GenTimeStep</span>, and <span class="Monospace">GenTimeNo</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="#" data-unresolved="1">TTR</a> function to convert a text in time format into a number.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">GenTimeUnit</td>
<td>Specifies the time unit for the step width.<div id="exp_GenTimeUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"year"</pre></donottranslate></td>
<td>Year</td></tr>
<tr><td width="150"><donottranslate><pre>"quarter"</pre></donottranslate></td>
<td>Quarter</td></tr>
<tr><td width="150"><donottranslate><pre>"month"</pre></donottranslate></td>
<td>Month</td></tr>
<tr><td width="150"><donottranslate><pre>"week"</pre></donottranslate></td>
<td>Week</td></tr>
<tr><td width="150"><donottranslate><pre>"day"</pre></donottranslate></td>
<td>Day</td></tr>
<tr><td width="150"><donottranslate><pre>"hour"</pre></donottranslate></td>
<td>Hour</td></tr>
<tr><td width="150"><donottranslate><pre>"minute"</pre></donottranslate></td>
<td>Minute</td></tr>
<tr><td width="150"><donottranslate><pre>"second"</pre></donottranslate></td>
<td>Second</td></tr>
<tr><td width="150"><donottranslate><pre>"millisecond"</pre></donottranslate></td>
<td>Millisecond</td></tr>
<tr><td width="150"><donottranslate><pre>"microsecond"</pre></donottranslate></td>
<td>Microsecond</td></tr>
</table>
</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If you specify a time unit of microseconds, the time format, for example, <span class="Monospace">#dd.mm.yyyy hh:nn:ss.ffff</span> can display a minimum of 100 microsecond steps.</td></tr></table>
</div></td></tr>
<tr><td width="150">GenTimeXBeg</td>
<td>Specifies the first value in a new time channel.<div id="exp_GenTimeXBeg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= GenTimeXBeg &lt;= +1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenTimeXEnd</td>
<td>Specifies the last value in a new time channel.<div id="exp_GenTimeXEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= GenTimeXEnd &lt;= +1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenTimeStep</td>
<td>Specifies the step width.<div id="exp_GenTimeStep">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">GenTimeMode</td>
<td>Specifies whether the last time value or the number of values limits the time channel.<div id="exp_GenTimeMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"StartStepEnd"</pre></donottranslate></td>
<td>Start/step width/end</td></tr>
<tr><td width="150"><donottranslate><pre>"StartStepNo"</pre></donottranslate></td>
<td>Start/step width/number</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenTimeNo</td>
<td>Specifies the number of values in the new time channel.<div id="exp_GenTimeNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= GenTimeNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
Range = "week"
oStartTime = dd.CreateTime(1999,11,20,0,0,0)
dStartTime = dd.ConvertTimeType (oStartTime,dd.eConvertDIAdemDateTime )
dd.ChnGenTime ("[]/GenTimeChn_dTime", Range, dStartTime, 0, 1, "StartStepNo", 10)
```

---

*Source: `ComOff/ChnGenTime.htm`*
