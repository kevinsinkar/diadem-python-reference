---
title: "ChnFullSpectrum"
description: "Calculates the full spectrum for a vibration analysis."
---

# ChnFullSpectrum

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFullSpectrum

Calculates the full spectrum for a vibration analysis.

## Signature

```python
return_value = dd.ChnFullSpectrum( FullSpectrumInputX , FullSpectrumInputY1 , FullSpectrumInputY2 , FullSpectrumWndFct, FullSpectrumWndCorrectType, FullSpectrumIntervalType, FullSpectrumNoOfIntervals, FullSpectrumIntervalLength)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FullSpectrumInputX</td>
<td>Specifies a time channel.<div id="exp_FullSpectrumInputX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">FullSpectrumInputY1</td>
<td>Specifies one or more input channels of sensor 1.<div id="exp_FullSpectrumInputY1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">FullSpectrumInputY2</td>
<td>Specifies one or more input channels of sensor 2.<div id="exp_FullSpectrumInputY2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">FullSpectrumWndFct</td>
<td>Specifies the window function.<div id="exp_FullSpectrumWndFct">
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
<tr><td width="150">FullSpectrumWndCorrectType</td>
<td>Specifies whether and how DIAdem corrects the damping effect of the window function on the amplitude.<div id="exp_FullSpectrumWndCorrectType">
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
<tr><td width="150">FullSpectrumIntervalType</td>
<td>Specifies the data volume of the calculation.<div id="exp_FullSpectrumIntervalType">
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
<tr><td width="150">FullSpectrumNoOfIntervals</td>
<td>Specifies the number of intervals.<div id="exp_FullSpectrumNoOfIntervals">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= FullSpectrumNoOfIntervals &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FullSpectrumIntervalLength</td>
<td>Specifies the number of values in an interval.<div id="exp_FullSpectrumIntervalLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= FullSpectrumIntervalLength &lt;= 2147483647</td></tr>
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

*Source: `ComOff/ChnFullSpectrum.htm`*
