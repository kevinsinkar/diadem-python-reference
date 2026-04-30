---
title: "ChnCorrelNCross"
description: "Calculates a normalized cross correlation, which means the result values are between -1 and 1."
---

# ChnCorrelNCross

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCorrelNCross

Calculates a normalized cross correlation, which means the result values are between -1 and 1.

## Signature

```python
return_value = dd.ChnCorrelNCross( XW , Y1 , Y2 , ResultChannel , ResultChannel , CorrelType, CorrelVal)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Use only the <a href="../chncorrelcross/">ChnCorrelCross</a> function for a normalized cross correlation and assign the value <span class="Monospace">1</span> to the <a href="../../../varoff/variables/correlnormalize/">CorrelNormalize</a> variable.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The values of the x-channel must be equidistant and monotonic increasing.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you perform a cross correlation in the frequency domain the number of values in each input channel should be a power of two. If not, DIAdem automatically selects the next lowest power of two for the calculation. The cross correlation in the time domain however uses all values of the input channels.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the y1-values.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel containing the y2-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that contains the x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that contains the y-values.</td></tr>
<tr><td width="150">CorrelType</td>
<td>Specifies whether DIAdem runs the calculation in the frequency domain or the time domain.<div id="exp_CorrelType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"TimeDomain"</pre></donottranslate></td>
<td>Time domain</td></tr>
<tr><td width="150"><donottranslate><pre>"FrequencyDomain"</pre></donottranslate></td>
<td>Frequency domain</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CorrelVal</td>
<td>Specifies the maximum shift of the signal, as a percentage of the channel length, for the correlation in the time domain.<div id="exp_CorrelVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= CorrelVal &lt;= 50</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnCorrelNCross.htm`*
