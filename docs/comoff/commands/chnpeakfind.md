---
title: "ChnPeakFind"
description: "Determines the local minimum and maximum values in a signal."
---

# ChnPeakFind

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPeakFind

Determines the local minimum and maximum values in a signal.

## Signature

```python
return_value = dd.ChnPeakFind( XW , Y , ResultChannel , ResultChannel , PeakNo, PeakType, PeakSort)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem ignores <a href="#" data-unresolved="1">NoValues</a> and their neighboring points during the peak search. The first value and the last value of a channel are not a local minimum or maximum.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the peaks.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the peaks.</td></tr>
<tr><td width="150">PeakNo</td>
<td>Specifies the maximum number of minimum or maximum values DIAdem searches for.<div id="exp_PeakNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>1 &lt;= PeakNo &lt;= <a href="../../../varoff/variables/peaknomax/">PeakNoMax</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">PeakType</td>
<td>Specifies whether DIAdem searches for minimum values or maximum values.<div id="exp_PeakType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Max.Peaks"</pre></donottranslate></td>
<td>Maximum peaks</td></tr>
<tr><td width="150"><donottranslate><pre>"Min.Peaks"</pre></donottranslate></td>
<td>Minimum peaks</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PeakSort</td>
<td>Specifies the order in which DIAdem searches for minimum values or maximum values.<div id="exp_PeakSort">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Time"</pre></donottranslate></td>
<td>Time</td></tr>
<tr><td width="150"><donottranslate><pre>"Amplitude"</pre></donottranslate></td>
<td>Amplitude</td></tr>
</table>
</td></tr>
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
dd.ChnResult = dd.ChnPeakFind("[1]/Time", "[1]/Speed", "/PeakX", "/PeakY", 5, "Max.Peaks", "Amplitude")
sOutput = "Results: " + "\r\n" + "Channelgroup: " + dd.ChnResult.Item(1).ChannelGroup.Name + "\r\n"
sOutput =  sOutput + "X-Channel: " + dd.ChnResult.Item(1).Name + "\r\n" + "Y-Channel: " + dd.ChnResult.Item(2).Name
print(sOutput)
```

---

*Source: `ComOff/ChnPeakFind.htm`*
