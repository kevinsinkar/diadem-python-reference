---
title: "ChnPeakDetect"
description: "Executes a peak value recognition, which means that DIAdem specifies the position, the second deduction, and the amplitude of the peaks and valleys in the input"
---

# ChnPeakDetect

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPeakDetect

Executes a peak value recognition, which means that DIAdem specifies the position, the second deduction, and the amplitude of the peaks and valleys in the input signal.

## Signature

```python
return_value = dd.ChnPeakDetect( XW , Y , ResultChannel , ResultChannel , PeakDetectType, PeakDetectThreshold, PeakDetectWidth)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the position of the found peaks.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the amplitude of the found peaks.</td></tr>
<tr><td width="150">PeakDetectType</td>
<td>Specifies the peak types.<div id="exp_PeakDetectType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Peaks"</pre></donottranslate></td>
<td>Peaks</td></tr>
<tr><td width="150"><donottranslate><pre>"Valleys"</pre></donottranslate></td>
<td>Valleys</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PeakDetectThreshold</td>
<td>Specifies the threshold up to which DIAdem ignores peaks and valleys. The adapted amplitude of the peaks must not be below the threshold. The adapted amplitude of the valleys must not be above the threshold value.<div id="exp_PeakDetectThreshold">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PeakDetectWidth</td>
<td>Specifies the number of successive points, which DIAdem uses for the adaptation with the least squares method. The value must be greater than or equal to three. The value should be at least half the width of the peaks or valleys and below that if the signals are noiseless. If the widths are large, you can decrease the apparent peak amplitudes and move the apparent position. If the data is noisy, this change is insignificant because the noise hides the actual peak. Select the smallest possible width, which is still large enough to preclude incorrect peak values created by noise.<div id="exp_PeakDetectWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>3 &lt;= PeakDetectWidth &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Specifies the result channels containing the position and the amplitude of the found peaks. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnResult = dd.ChnPeakDetect("[1]/Time", "[1]/Speed", "/Position", "/Amplitude", "Peaks", 0, 3)
sOutput = "Results: " + "\r\n" + "Channelgroup: " + dd.ChnResult.Item(1).ChannelGroup.Name + "\r\n"
sOutput =  sOutput + "X-Channel: " + dd.ChnResult.Item(1).Name + "\r\n" + "Y-Channel: " + dd.ChnResult.Item(2).Name
print(sOutput)
```

---

*Source: `ComOff/ChnPeakDetect.htm`*
