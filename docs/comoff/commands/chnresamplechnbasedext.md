---
title: "ChnResampleChnBasedExt"
description: "Maps several signals onto a common interpolation channel."
---

# ChnResampleChnBasedExt

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnResampleChnBasedExt

Maps several signals onto a common interpolation channel.

## Signature

```python
return_value = dd.ChnResampleChnBasedExt( XW , ChnList, SamplingPointChn, ResampleMappingMode, ResampleAntiAliasingFilter, ResampleInterpolateNovalues, [ResampleInterpolationMethod])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values. If all y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">SamplingPointChn</td>
<td>Specifies the data channel containing the interpolation points.<div id="exp_SamplingPointChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
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
<td>Contains the result channels with the y-values converted to the interpolation points. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.<br attr="ext"/>The names of the result channels are composed of <span class="Monospace">ResampledSignal_</span> and the respective name of the y-channel.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyChannelList = dd.Data.GetChannels("[4]/T*")
oMyX1Channel = dd.Data.Root.ChannelGroups(1).Channels(3)
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnResampleChnBasedExt(oMyXChannel, oMyChannelList, oMyX1Channel, "Automatic", False, False, "Akima")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[4]/T*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnResampleChnBasedExt("[1]/[1]", oMyChannelList, "[1]/[3]", "Automatic", False, False, "Akima")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnResampleChnBasedExt.htm`*
