---
title: "XOffsetCalc"
description: "Determines the maximum offset of a cross correlation."
---

# XOffsetCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: XOffsetCalc

Determines the maximum offset of a cross correlation.

## Signature

```python
dd.XOffsetCalc( XW , Y1 , Y2 , XOffsetType, XOffsetVal)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition DIAdem saves the calculation results in the following custom properties of the input channels: <span class="Monospace">Result~XOffset~CorrelationCoefficient</span>, <span class="Monospace">Result~XOffset~DeltaN</span>, and <span class="Monospace">Result~XOffset~DeltaT</span>.</td></tr></table>
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
<tr><td width="150">XOffsetType</td>
<td>Specifies whether DIAdem runs a cross correlation calculation in the frequency domain or the time domain.<div id="exp_XOffsetType">
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
<tr><td width="150">XOffsetVal</td>
<td>Specifies the maximum shift of the signal, as a percentage of the channel length, for the cross correlation in the time domain.<div id="exp_XOffsetVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= XOffsetVal &lt;= 50</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">XOffsetDeltaT</td><td>Receives in a cross correlation the absolute time value of the maximum offset of the second xy-curve to the first xy-curve. If the <span class="Monospace">XOffsetDeltaT</span> variable receives, for example, the value <span class="Monospace">4</span>, you must move the second xy-curve <span class="Monospace">-4</span> in x-direction so that the y-values correspond.<div id="exp_XOffsetDeltaT">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-1E301 &lt;= XOffsetDeltaT &lt;= 1E301</td></tr>
</table>
</div></td></tr>
<tr><td width="150">XOffsetDeltaN</td><td>Receives in a cross correlation the number of values of the maximum offset of the second xy-curve to the first xy-curve. If the <span class="Monospace">XOffsetDeltaN</span> variable receives, for example, the value <span class="Monospace">4</span>, you must move the second y-channel up four values in the channel table so that the y-values correspond.<div id="exp_XOffsetDeltaN">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= XOffsetDeltaN &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">XOffsetCorrCoefficient</td><td>Receives the coefficients of the cross correlation.<div id="exp_XOffsetCorrCoefficient">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= XOffsetCorrCoefficient &lt;= 1</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/XOffsetCalc.htm`*
