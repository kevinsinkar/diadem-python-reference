---
title: "ChnResampleFreqBased"
description: "Maps a signal onto a new sampling rate."
---

# ChnResampleFreqBased

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnResampleFreqBased

Maps a signal onto a new sampling rate.

## Signature

```python
return_value = dd.ChnResampleFreqBased( XW , Y , ResultChannel , SampleFrequency, ResampleMappingMode, ResampleAntiAliasingFilter, ResampleInterpolateNovalues, [ResampleInterpolationMethod])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the converted y-values.</td></tr>
<tr><td width="150">SampleFrequency</td>
<td>Specifies the sampling rate of the result channel in Hertz.<div id="exp_SampleFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SampleFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ResampleMappingMode</td>
<td>Specifies the mapping mode for the resampling.<div id="exp_ResampleMappingMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"Stair"</pre></donottranslate></td>
<td>Stairs</td></tr>
<tr><td width="150"><donottranslate><pre>"Analog"</pre></donottranslate></td>
<td>Analog</td></tr>
</table>
</td></tr>
</table>
<p>If you select the <span class="Monospace">"Analog”</span> setting, DIAdem interpolates the signal according to the settings of the <span class="Monospace">ResampleInterpolationMethod</span> variable. If you select <span class="Monospace">"Stair"</span>, DIAdem retains the last known value until the y-input channel receives a new value. For the <span class="Monospace">"Automatic”</span> setting, the resampling function specifies the display type as follows: If in the y input channel at least n/2-1 of the values correspond to their predecessor or if the y-input channel only contains integer values, DIAdem uses the stairs mapping mode. If both conditions are not fulfilled, DIAdem uses the analog mapping mode.</p>
<p>DIAdem saves the specified mapping mode as a custom property called <span class="Monospace">NI_display_mode</span> in the result channels. If the automatic mode does not return the required mapping mode, set the <span class="Monospace">NI_display_mode</span> channel property before the resampling. In <span class="Monospace">"Automatic"</span> mapping mode DIAdem uses the mapping mode specified in this property.</p>
</div></td></tr>
<tr><td width="150">ResampleAntiAliasingFilter</td>
<td>Specifies that DIAdem filters the y input channel. The default value of the variable is <span class="Monospace">FALSE</span>, so that DIAdem does not filter the input channel.<div id="exp_ResampleAntiAliasingFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p>DIAdem only filters the y input channel if the new sampling rate is smaller than half of the original sampling frequency. As a filter function DIAdem uses a two-step Butterworth filter, which filters 20% below half of the new sampling frequency and corrects the start offset.</p>
</div></td></tr>
<tr><td width="150">ResampleInterpolateNovalues</td>
<td>Specifies that DIAdem replaces the NoValues in the y-values by interpolating the neighboring points. The default value of the variable is <span class="Monospace">FALSE</span> so that DIAdem does not replace NoValues.<div id="exp_ResampleInterpolateNovalues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ResampleInterpolationMethod]</td>
<td>Specifies how DIAdem interpolates the y-channels if the <span class="Monospace">ResampleMappingMode</span> variable has the value <span class="Monospace">"Analog"</span>. As a default, the <span class="Monospace">ResampleInterpolationMethod</span> variable has the value <span class="Monospace">"Akima"</span>, which means that DIAdem interpolates the signal with Akima subsplines if you do not specify the value.<div id="exp_ResampleInterpolationMethod">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Akima"</pre></donottranslate></td>
<td>Akima</td></tr>
<tr><td width="150"><donottranslate><pre>"Linear"</pre></donottranslate></td>
<td>Linear</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel with the y-values converted to the interpolation points. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.ChnResampleFreqBased(oMyXChannel, oMyYChannel, "Results/Resampled", 1, "Automatic", False, False, "Akima")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyResultChn = dd.ChnResampleFreqBased("[1]/[1]", "[1]/[2]", "Results/Resampled", 1, "Automatic", False, False, "Akima")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnResampleFreqBased.htm`*
