---
title: "ChnGenSignal"
description: "Generates a new channel with a given signal form."
---

# ChnGenSignal

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGenSignal

Generates a new channel with a given signal form.

## Signature

```python
return_value = dd.ChnGenSignal(GenSignalFunction, GenSignalNoOfValues, GenSignalSamplingRate, ResultChannel , GenSignalFrequency, GenSignalAmplitude, GenSignalPhaseShift, GenSignalOffset, GenSignalTimeUnit, GenSignalUnit, GenSignalDutyCycle)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">GenSignalFunction</td>
<td>Specifies the signal form of the generated signal.<div id="exp_GenSignalFunction">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Sine"</pre></donottranslate></td>
<td>Sine</td></tr>
<tr><td width="150"><donottranslate><pre>"Rectangle"</pre></donottranslate></td>
<td>Rectangle</td></tr>
<tr><td width="150"><donottranslate><pre>"Triangle"</pre></donottranslate></td>
<td>Triangle</td></tr>
<tr><td width="150"><donottranslate><pre>"Noise"</pre></donottranslate></td>
<td>Noise</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalNoOfValues</td>
<td>Specifies the number of values in the generated channel.<div id="exp_GenSignalNoOfValues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>1 &lt;= GenSignalNoOfValues &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalSamplingRate</td>
<td>Specifies the sampling rate of the generated channel in Hertz, and thus the number of values to be generated for each period.<div id="exp_GenSignalSamplingRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalSamplingRate &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body"><em>GenSignalSamplingRate</em> should be at least twice <em>GenSignalFrequency</em>. You do not need this variable for the signal form <span class="Monospace">noise</span>.</p>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the name of the result channel.</td></tr>
<tr><td width="150">GenSignalFrequency</td>
<td>Specifies the frequency of the generated channel in Hertz.<div id="exp_GenSignalFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalFrequency &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">You do not need this variable for the signal form <span class="Monospace">noise</span>.</p>
</div></td></tr>
<tr><td width="150">GenSignalAmplitude</td>
<td>Specifies the amplitude of the generated channel.<div id="exp_GenSignalAmplitude">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalAmplitude &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalPhaseShift</td>
<td>Specifies the phase offset of the generated signals as a percentage of a period.<div id="exp_GenSignalPhaseShift">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalPhaseShift &lt;= 100.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="body">You do not need this variable for the signal form <span class="Monospace">noise</span>.</p>
</div></td></tr>
<tr><td width="150">GenSignalOffset</td>
<td>Specifies the amplitude offset of the generated channel.<div id="exp_GenSignalOffset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalOffset &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalTimeUnit</td>
<td>Specifies the unit of the time values of the generated signal.<div id="exp_GenSignalTimeUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"ms"</pre></donottranslate></td>
<td>ms</td></tr>
<tr><td width="150"><donottranslate><pre>"s"</pre></donottranslate></td>
<td>s</td></tr>
<tr><td width="150"><donottranslate><pre>"min"</pre></donottranslate></td>
<td>min</td></tr>
<tr><td width="150"><donottranslate><pre>"h"</pre></donottranslate></td>
<td>h</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalUnit</td>
<td>Specifies the unit of the amplitude values of the generated channel.<div id="exp_GenSignalUnit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 10 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GenSignalDutyCycle</td>
<td>Specifies the symmetry of the generated channel. The value range of the clock ratio is between 0 and 100%. A symmetric signal form has a clock ratio of 50%.<div id="exp_GenSignalDutyCycle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= GenSignalDutyCycle &lt;= 100.0<br attr="ext"/>Access: Read/Write</td></tr>
</table>You do not need this variable for the signal forms <span class="Monospace">Sine</span> and <span class="Monospace">Noise</span>.</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel as <a href="#" data-unresolved="1">waveform channel</a>. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
if dd.Data.Root.ChannelGroups.Exists("GenSignal") :
    dd.Data.Root.ChannelGroups.Remove("GenSignal")

oMyGroup = dd.Data.Root.ChannelGroups.Add("GenSignal")
oMyGenSigChn = oMyGroup.Channels.Add("GeneratedSignal", dd.DataTypeChnFloat64)
dd.ChnGenSignal("Rectangle", 1024, 100, oMyGenSigChn, 3, 10, 0, 0, "s", "V", 50)
dd.MsgboxDisp("Result channel: " + oMyGroup.Name + "/" + oMyGenSigChn.Name)
```

```python
oMyResultChn = dd.ChnGenSignal("Rectangle", 1024, 100, "/GeneratedSignal", 3, 10, 0, 0, "s", "V", 50)
dd.MsgboxDisp("Result channel: " + oMyResultChn.Item(1).ChannelGroup.Name+ "/"+oMyResultChn.Item(1).Name)
```

---

*Source: `ComOff/ChnGenSignal.htm`*
