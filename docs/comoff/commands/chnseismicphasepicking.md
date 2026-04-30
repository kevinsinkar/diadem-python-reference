---
title: "ChnSeismicPhasePicking"
description: "Specifies the arrival times of the primary waves (P waves) and the secondary waves (S waves) of a seismic event. DIAdem calculates P-waves with the moving avera"
---

# ChnSeismicPhasePicking

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSeismicPhasePicking

Specifies the arrival times of the primary waves (P waves) and the secondary waves (S waves) of a seismic event. DIAdem calculates P-waves with the moving averages short-term average (STA) and long-term average (LTA).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds. If all associated y-channels are waveform channels and you do not specify the xw-channel, DIAdem uses the x-part of the associated waveform channels.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the first data channel with horizontal values, for example, in north-south direction.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the second data channel with horizontal values, for example, in east-west direction.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with vertical values.</td></tr>
<tr><td width="150">SeismicSTAWidth</td>
<td>Specifies the time span for calculating the short-term average (STA) in seconds. When calculating the STA mean value, outliers such as a single impact have only a minor effect, while persistently high amplitudes of a P wave result in a high mean value.<div id="exp_SeismicSTAWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= SeismicSTAWidth &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SeismicLTAWidth</td>
<td>Specifies the time span for calculating the long-term average (LTA) in seconds. The LTA corresponds with the background noise of a seismic signal.<div id="exp_SeismicLTAWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= SeismicLTAWidth &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SeismicSignalNoiseRatio</td>
<td>Specifies the ratio of short-term average to long-term average. The ratio of the two mean values must exceed a threshold for DIAdem to detect the P waves of a seismic event.<div id="exp_SeismicSignalNoiseRatio">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>1 &lt;= SeismicSignalNoiseRatio &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SeismicPPhaseDuration</td>
<td>Specifies the minimum peak duration in seconds for DIAdem to recognize the peaks as P-waves of a seismic event.<div id="exp_SeismicPPhaseDuration">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= SeismicPPhaseDuration &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SeismicSPhasePickMode</td>
<td>Specifies whether DIAdem uses the largest peak or the first peak to determine the S phase of a seismic event.<div id="exp_SeismicSPhasePickMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FirstPeak"</pre></donottranslate></td>
<td>First peak</td></tr>
<tr><td width="150"><donottranslate><pre>"LargestPeak"</pre></donottranslate></td>
<td>Largest peak</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If you use the largest peak, DIAdem defines the start of the S phase as the last local minimum before the global maximum. In addition, the local minimum must be below the standard deviation. Select this setting if the surface waves are not very pronounced, which means the measuring station is relatively far away from the epicenter. If you use the first peak, DIAdem defines the start of the S phase as the value from which the signal exceeds the standard deviation for the minimum duration of the P phase. Select this setting when surface waves trigger large peaks.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value in a one-dimensional array is <span class="Monospace">True</span>, DIAdem findes P-waves or S-waves and <span class="Monospace">False</span> if DIAdem does not find any P or S waves. The return value is a <a href="#" data-unresolved="1">Variant variable</a> type.<table class="Borderless">
<tr>
<th class="Bordered" style="width: 100"> </th>
<th class="Bordered" style="width: 100">Return value</th>
</tr>
<tr>
<th class="Bordered" style="width: 100">Line 0</th>
<td class="bordered" style="text-align:center">P-waves found</td>
</tr>
<tr>
<th class="Bordered" style="width: 100">Line 1</th>
<td class="bordered" style="text-align:center">S-waves found</td>
</tr></table>
</td></tr>
</table>
</div>

## Python example

```python
oMyGroup = dd.Data.Root.ChannelGroups(1)
oMyY1Chn = oMyGroup.Channels(1)
oMyY2Chn = oMyGroup.Channels(2)
oMyY3Chn = oMyGroup.Channels(3)
sPhases = dd.ChnSeismicPhasePicking("", oMyY1Chn, oMyY2Chn, oMyY3Chn, 0.1, 10, 15, 1.5, "LargestPeak")
if sPhases(0) and sPhases(1) :
    dd.MsgBoxDisp("P Phase Arrival: "+ dd.SeismicPArrivals(0,1) + "\r\n" + "S Phase Arrival: " + dd.SeismicSArrivals(0,1))
elif sPhases(0) :
    dd.MsgBoxDisp("P Phase Arrival: "+ dd.SeismicPArrivals(0,1))
else:
    dd.MsgBoxDisp("No seismic phases detected")
```

```python
sPhases = dd.ChnSeismicPhasePicking("", "[1]/Horizontal 1", "[1]/Horizontal 2", "[1]/Vertical", 0.1, 10, 15, 1.5, "LargestPeak")
if sPhases(0) and sPhases(1) :
    dd.MsgBoxDisp("P Phase Arrival: "+ dd.SeismicPArrivals(0,1) + "\r\n" + "S Phase Arrival: " + dd.SeismicSArrivals(0,1))
elif sPhases(0) :
    dd.MsgBoxDisp("P Phase Arrival: "+ dd.SeismicPArrivals(0,1))
else:
    dd.MsgBoxDisp("No seismic phases detected")
```

---

*Source: `ComOff/ChnSeismicPhasePicking.htm`*
