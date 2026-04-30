---
title: "ChnPulseDetection"
description: "Evaluates the tachometer signals. At regular intervals a tachometer signal contains pulses measured by sensors on a shaft."
---

# ChnPulseDetection

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPulseDetection

Evaluates the tachometer signals. At regular intervals a tachometer signal contains pulses measured by sensors on a shaft.

## Signature

```python
return_value = dd.ChnPulseDetection( PulseInputX , PulseInputY , PulseDetResultType, PulseDetThresholdType, PulseDetThresholdValue, PulseDetPulseRevolution, PulseDetHysteresisType, PulseDetHysteresisValue, PulseDetPulseWidth, PulseDetSlope, PulseDetInterpolMissValues)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">PulseInputX</td>
<td>Specifies the data channel containing the time values of the tachometer channel.<div id="exp_PulseInputX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">PulseInputY</td>
<td>Specifies the data channels with the tachometer signals.<div id="exp_PulseInputY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">PulseDetResultType</td>
<td>Specifies the results of the tachometer signal evaluation.<div id="exp_PulseDetResultType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"PulseStartTime"</pre></donottranslate></td>
<td>Pulse start times</td></tr>
<tr><td width="150"><donottranslate><pre>"PulseDetectedRevolution"</pre></donottranslate></td>
<td>Rpm</td></tr>
<tr><td width="150"><donottranslate><pre>"PulseStartChnLine"</pre></donottranslate></td>
<td>Index pulse start times</td></tr>
<tr><td width="150"><donottranslate><pre>"PulseStartDetected"</pre></donottranslate></td>
<td>Pulse start status channel</td></tr>
<tr><td width="150"><donottranslate><pre>"PulseNoOperation"</pre></donottranslate></td>
<td>No evaluation</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetThresholdType</td>
<td>Specifies whether DIAdem interprets the threshold value as an absolute numeric value or as a percentage. If you select <span class="Monospace">Percentage</span>, the threshold refers to the range between the global minimum and maximum of the current tachometer channel.<div id="exp_PulseDetThresholdType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Absolute"</pre></donottranslate></td>
<td>Absolute</td></tr>
<tr><td width="150"><donottranslate><pre>"Percentage"</pre></donottranslate></td>
<td>Percentage</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetThresholdValue</td>
<td>Specifies the threshold which the signal must exceed in order to be validated as a pulse.<div id="exp_PulseDetThresholdValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetPulseRevolution</td>
<td>Specifies the number of pulses for one revolution.<div id="exp_PulseDetPulseRevolution">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= PulseDetPulseRevolution &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetHysteresisType</td>
<td>Specifies whether DIAdem interprets the hysteresis as an absolute numeric value or as a percentage. If you select <span class="Monospace">Percentage</span>, the hysteresis refers to the range between the global minimum and maximum of the current tachometer channel.<div id="exp_PulseDetHysteresisType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Absolute"</pre></donottranslate></td>
<td>Absolute</td></tr>
<tr><td width="150"><donottranslate><pre>"Percentage"</pre></donottranslate></td>
<td>Percentage</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetHysteresisValue</td>
<td>Specifies the minimum range in addition to the threshold, which the pulse must have. This is to prevent disturbances.<div id="exp_PulseDetHysteresisValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetPulseWidth</td>
<td>Specifies the minimum width of a pulse. The default value is <span class="Monospace">2</span>, which means that two consecutive tachometer values must reach the threshold for a pulse to be detected.<div id="exp_PulseDetPulseWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= PulseDetPulseWidth &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetSlope</td>
<td>Specifies whether the pulse must increase or decrease.<div id="exp_PulseDetSlope">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Rising"</pre></donottranslate></td>
<td>Increasing</td></tr>
<tr><td width="150"><donottranslate><pre>"Falling"</pre></donottranslate></td>
<td>Decreasing</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseDetInterpolMissValues</td>
<td>Specifies whether DIAdem uses linear interpolation to add missing pulses.<div id="exp_PulseDetInterpolMissValues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= PulseDetInterpolMissValues &lt;= 1</td></tr>
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

---

*Source: `ComOff/ChnPulseDetection.htm`*
