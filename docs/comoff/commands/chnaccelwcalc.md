---
title: "ChnAccelWCalc"
description: "Evaluates an acceleration signal with a frequency weighting filter."
---

# ChnAccelWCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnAccelWCalc

Evaluates an acceleration signal with a frequency weighting filter.

## Signature

```python
dd.ChnAccelWCalc( XW , Y , AWFiltType, AWRMSRunning, AWRMSTime, AWRedFactor)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For hand-arm vibrations, the sampling frequency must be higher than 1000 Hz, in other cases it must be higher than 200 Hz.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
<tr><td width="150">AWFiltType</td>
<td>Specifies the frequency weighting filter for time-related body and hand-arm vibrations in accordance with ISO 2631-1 and VDI 2057-1,2.<div id="exp_AWFiltType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"WK"</pre></donottranslate></td>
<td>Wk: Vertical whole-body vibration z-axis (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WD"</pre></donottranslate></td>
<td>Wd: Horizontal whole-body vibration x-axis or y-axis (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WF"</pre></donottranslate></td>
<td>Wf: Low-frequency vertical whole-body vibration z-axis (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WC"</pre></donottranslate></td>
<td>Wc: Horizontal whole-body vibration x-axis (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WE"</pre></donottranslate></td>
<td>We: Rotating whole-body vibration (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WJ"</pre></donottranslate></td>
<td>Wj: Vertical head vibration (ISO 2631-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"WB"</pre></donottranslate></td>
<td>Wb: Vertical whole-body vibration z-axis (ISO 2631-4)</td></tr>
<tr><td width="150"><donottranslate><pre>"WH"</pre></donottranslate></td>
<td>Wh: Hand-arm vibration (ISO 5349-1)</td></tr>
<tr><td width="150"><donottranslate><pre>"W.B.combined"</pre></donottranslate></td>
<td>W.B.combined: Vibration on non-specific posture (DIN 45671-1/VDI 2057-1)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AWRMSRunning</td>
<td>Specifies whether DIAdem calculates the floating RMS for the frequency-weighted acceleration.<div id="exp_AWRMSRunning">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">AWRMSTime</td>
<td>Specifies the time constant for mean calculations, in seconds.<div id="exp_AWRMSTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= AWRMSTime &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AWRedFactor</td>
<td>Specifies how many values DIAdem groups into one result value in a frequency-weighted acceleration.<div id="exp_AWRedFactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= AWRedFactor &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnAccelWCalc.htm`*
