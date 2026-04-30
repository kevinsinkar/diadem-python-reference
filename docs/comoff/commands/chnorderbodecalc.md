---
title: "ChnOrderBodeCalc"
description: "Uses the sensor signals to calculate the amplitudes and phases for each order for a Bode diagram."
---

# ChnOrderBodeCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnOrderBodeCalc

Uses the sensor signals to calculate the amplitudes and phases for each order for a Bode diagram.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Due to a change in the calculation, the amplitude values of the result channels in DIAdem 2015 were greater than the calculation results of the current version by a factor of four.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OrderBodeInputX</td>
<td>Specifies a time channel.<div id="exp_OrderBodeInputX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">OrderBodeInputY</td>
<td>Specifies one or more channels with the sensor signals. The sensor channels must not contain <a href="../../../varoff/variables/nv/">NoValues</a>. The number of signal channels must be the same as the number of pulse time channels.<div id="exp_OrderBodeInputY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">OrderBodeInputPulseTime</td>
<td>Specifies one or more channels with the pulse start times. The pulse start times are the intervals between the individual pulses, which you can specify with the <a href="#" data-unresolved="1">Pulse detection</a>.<div id="exp_OrderBodeInputPulseTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">OrderBodeWndFct</td>
<td>Specifies the window function.<div id="exp_OrderBodeWndFct">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Rectangle"</pre></donottranslate></td>
<td>Rectangle</td></tr>
<tr><td width="150"><donottranslate><pre>"Hanning"</pre></donottranslate></td>
<td>Hanning</td></tr>
<tr><td width="150"><donottranslate><pre>"Hamming"</pre></donottranslate></td>
<td>Hamming</td></tr>
<tr><td width="150"><donottranslate><pre>"Blackman"</pre></donottranslate></td>
<td>Blackman</td></tr>
<tr><td width="150"><donottranslate><pre>"FlatTop"</pre></donottranslate></td>
<td>FlatTop</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeWndCorrectType</td>
<td>Specifies whether and how DIAdem corrects the damping effect of the window function on the amplitude.<div id="exp_OrderBodeWndCorrectType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"No"</pre></donottranslate></td>
<td>No</td></tr>
<tr><td width="150"><donottranslate><pre>"Periodic"</pre></donottranslate></td>
<td>Periodic</td></tr>
<tr><td width="150"><donottranslate><pre>"Random"</pre></donottranslate></td>
<td>Random</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeIntervalType</td>
<td>Specifies the data amount of the calculation.<div id="exp_OrderBodeIntervalType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NoOfIntervals"</pre></donottranslate></td>
<td>Number of intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"IntervalLength"</pre></donottranslate></td>
<td>Length of the intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"All"</pre></donottranslate></td>
<td>All</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeNoOfIntervals</td>
<td>Specifies the number of intervals.<div id="exp_OrderBodeNoOfIntervals">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OrderBodeNoOfIntervals &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeIntervalLength</td>
<td>Specifies the number of values in an interval.<div id="exp_OrderBodeIntervalLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OrderBodeIntervalLength &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeCalcOrder</td>
<td>Specifies the orders of the curves to be calculated.<div id="exp_OrderBodeCalcOrder">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeBandwidthBegin</td>
<td>Specifies the start value of the bandwidth of an order.<div id="exp_OrderBodeBandwidthBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeBandwidthEnd</td>
<td>Specifies the end value of the bandwidth of an order.<div id="exp_OrderBodeBandwidthEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeRunoutCompAmplitudeRef</td>
<td>Specifies the value for the runout correction of the amplitude which DIAdem subtracts from the amplitude calculated for the first order.<div id="exp_OrderBodeRunoutCompAmplitudeRef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OrderBodeRunoutCompPhaseRef</td>
<td>Specifies the value for the runout correction of the phase which DIAdem subtracts from the phase calculated for the first order.<div id="exp_OrderBodeRunoutCompPhaseRef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value. For every N order and for every time interval, DIAdem generates the result channels <span class="Monospace">BodeAmplitudeNOrder</span> with the amplitudes and <span class="Monospace">BodePhaseNOrder</span> with the phases. The result channel <span class="Monospace">BodeSpeed</span> contains the rpm and <span class="Monospace">BodeTime</span> the time values of the reference axis. The calculated amplitudes only depend on the bandwidth and not on the order. The calculated phases, on the other hand, also depend on the order.<br attr="ext"/>Unlike the <span class="Monospace">ChnOrderBodeCalc</span> command, the <a href="../chnpulsedetection/">ChnPulseDetection</a><span class="Monospace"></span> command calculates the specific rpm for each revolution and not just average rpm over the selected interval. If the selected interval does not contain pulses, the <span class="Monospace">ChnOrderBodeCalc</span> command cannot calculate rpm. To select the intervals appropriately, you can use the <span class="Monospace">PulseStartDetected</span> pulse start status channel of the <span class="Monospace">ChnPulseDetection</span> command.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnOrderBodeCalc.htm`*
