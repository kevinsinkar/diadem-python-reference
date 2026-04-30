---
title: "ChnResampleFreqBasedXOffsetCalc3"
description: "Uses a synchronization channel to map three measurements on a new sampling rate."
---

# ChnResampleFreqBasedXOffsetCalc3

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnResampleFreqBasedXOffsetCalc3

Uses a synchronization channel to map three measurements on a new sampling rate.

## Signature

```python
dd.ChnResampleFreqBasedXOffsetCalc3( XW , Y , ChnList, XOffset, XW , Y1 , ChnList1, XOffset1, XW , Y2 , ChnList2, XOffset2, AutoTimeChn, XOffsetMode, SampleFrequency, [ResampleMappingMode], [ResampleAntiAliasingFilter], [ResampleInterpolateNovalues], [ResampleCorrelationMode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the time channel of the first measurement. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the synchronization channel of the first measurement.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">XOffset</td>
<td>Specifies the offset for the first synchronization channel.<div id="exp_XOffset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>XW</em></td>
<td>Specifies the time channel of the second measurement. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the synchronization channel of the second measurement.</td></tr>
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">XOffset1</td>
<td>Specifies the offset for the second synchronization channel.<div id="exp_XOffset1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>XW</em></td>
<td>Specifies the time channel of the third measurement. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the synchronization channel of the third measurement.</td></tr>
<tr><td width="150">ChnList2</td>
<td>Specifies one or more channels.<div id="exp_ChnList2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">XOffset2</td>
<td>Specifies the offset for the third synchronization channel.<div id="exp_XOffset2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">AutoTimeChn</td>
<td>Specifies whether DIAdem uses the first channel of a channel group as the time channel or whether you specify the time channel. If the value is <span class="Monospace">TRUE</span>, DIAdem uses the first channel of a channel group as the time channel. If the input channels are waveform channels, DIAdem uses the time part of the waveform.<div id="exp_AutoTimeChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XOffsetMode</td>
<td>Specifies whether you set the offset or whether DIAdem automatically sets the offset.<div id="exp_XOffsetMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"Custom"</pre></donottranslate></td>
<td>Adjusted</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SampleFrequency</td>
<td>Specifies the sampling rate of the result channel in Hertz.<div id="exp_SampleFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SampleFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ResampleMappingMode]</td>
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
<tr><td width="150">[ResampleAntiAliasingFilter]</td>
<td>Specifies that DIAdem filters the y input channel. The default value of the variable is <span class="Monospace">FALSE</span>, so that DIAdem does not filter the input channel.<div id="exp_ResampleAntiAliasingFilter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p>DIAdem only filters the y input channel if the new sampling rate is smaller than half of the original sampling frequency. As a filter function DIAdem uses a two-step Butterworth filter, which filters 20% below half of the new sampling frequency and corrects the start offset.</p>
</div></td></tr>
<tr><td width="150">[ResampleInterpolateNovalues]</td>
<td>Specifies that DIAdem replaces NoValues in the y input channel by interpolating the neighbor points. The default value of the variable is <span class="Monospace">FALSE</span> so that DIAdem does not replace NoValues.<div id="exp_ResampleInterpolateNovalues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ResampleCorrelationMode]</td>
<td>Specifies whether DIAdem runs the cross correlation calculation in the frequency domain or the time domain. The default value of the variable is <span class="Monospace">“FrequencyDomain”</span>, so that DIAdem executes the calculation in the frequency domain.<div id="exp_ResampleCorrelationMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FrequencyDomain"</pre></donottranslate></td>
<td>Frequency domain</td></tr>
<tr><td width="150"><donottranslate><pre>"TimeDomain"</pre></donottranslate></td>
<td>Time domain</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnResampleFreqBasedXOffsetCalc3.htm`*
