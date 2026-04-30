---
title: "ChnMapLinCalcExt"
description: "Maps several signals onto a new common x-value range."
---

# ChnMapLinCalcExt

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMapLinCalcExt

Maps several signals onto a new common x-value range.

## Signature

```python
return_value = dd.ChnMapLinCalcExt( XW , ChnList, X1 , MapLinNovInterp, MapLinExtType, MapLinBdryVal, MapLinFctType, [MapLinInnerVal])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For digital functions such as spikes and stairs the maximum step width of the new x-range must be smaller than half of the minimum step width of the original x-range. This way you can avoid level changes. DIAdem also can assign two values Y(Xa), Y(Xb) to the same interpolation value X1. In this case DIAdem takes the value (y(xa) or y(xb)) of which the interpolation point (xa or xb) is closest to the new interpolation value x1. If both of the original interpolation points (xa and xb) are the same distance from the new interpolation value (x1), the y-value of the lower interpolation point is the result.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signals. If all y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel with the interpolation points of the new x-range.</td></tr>
<tr><td width="150">MapLinNovInterp</td>
<td>Specifies whether DIAdem replaces NoValues in the y-values.<div id="exp_MapLinNovInterp">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">You can replace NoValues that occur during the linear mapping. If you have a analog function, DIAdem runs a linear interpolation. If you have a spike function, DIAdem replaces the NoValues with zeros. If you have a stair function, DIAdem continues the level. If you do not replace NoValues, DIAdem uses the NoValues in the map.</p>
</div></td></tr>
<tr><td width="150">MapLinExtType</td>
<td>Specifies the extrapolation type that DIAdem uses to extend mapping outside the original x-range.<div id="exp_MapLinExtType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"const. value"</pre></donottranslate></td>
<td>Constant value</td></tr>
<tr><td width="150"><donottranslate><pre>"Y[bound.value]"</pre></donottranslate></td>
<td>Y[boundary value]</td></tr>
<tr><td width="150"><donottranslate><pre>"f[bound.slope]"</pre></donottranslate></td>
<td>f[boundary slope]</td></tr>
</table>
</td></tr>
</table>
<p class="Body"><strong>Valid Settings</strong></p>
<table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse">
<tr>
<td width="150"><span class="Monospace">const value</span></td>
<td>If the original x-range is exceeded, DIAdem continues the interpolation curve with a constant value. Specify the <a href="../../../varoff/variables/maplinbdryval/">Constant</a> with the variable <a href="../../../varoff/variables/maplinbdryval/">MapLinBdryVal</a>.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">Y[bound.value]</span></td>
<td>If the original x-range is exceeded, DIAdem continues the interpolation curve with a constant. DIAdem continues analog functions with the respective boundary value. DIAdem continues spike and stair functions with the value <span class="Monospace">0</span>.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">f[bound.slope]</span></td>
<td>If the original x-range is exceeded, DIAdem continues the interpolation curve linear. The slope of the straight line corresponds to the slope of the respective boundary value. You only can use this setting for analog functions.</td>
</tr>
</table>
<p>
</p></div></td></tr>
<tr><td width="150">MapLinBdryVal</td>
<td>Specifies the constant value for extrapolation with a constant value.<div id="exp_MapLinBdryVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">You can continue a linear mapping beyond the original x-range. If you select a constant numeric value as extrapolation type to continue the mapping, you use the <span class="Monospace">MapLinBdryVal</span> variable to specify the value of the constant. You also can select <span class="Monospace">NoValue</span> as the constant.</p>
</div></td></tr>
<tr><td width="150">MapLinFctType</td>
<td>Specifies the type of function that is to be mapped.<div id="exp_MapLinFctType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"analogue"</pre></donottranslate></td>
<td>Analog</td></tr>
<tr><td width="150"><donottranslate><pre>"Spike"</pre></donottranslate></td>
<td>Spikes</td></tr>
<tr><td width="150"><donottranslate><pre>"Stairs"</pre></donottranslate></td>
<td>Stairs</td></tr>
<tr><td width="150"><donottranslate><pre>"Stairs/analogue"</pre></donottranslate></td>
<td>Stairs/analog</td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
</table>
</td></tr>
</table>
<p class="Body">DIAdem maps analog functions with linear interpolations. DIAdem maps spike and stair functions by assigning spikes or slopes to the next interpolation points in the new x-range.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For digital functions such as spikes and stairs the maximum step width of the new x-range must be smaller than half of the minimum step width of the original x-range. This way you can avoid level changes. DIAdem also can assign two values Y(Xa), Y(Xb) to the same interpolation value X1. In this case DIAdem takes the value (y(xa) or y(xb)) of which the interpolation point (xa or xb) is closest to the new interpolation value x1. If both of the original interpolation points (xa and xb) are the same distance from the new interpolation value (x1), the y-value of the lower interpolation point is the result.</td></tr></table>
</div></td></tr>
<tr><td width="150">[MapLinInnerVal]</td>
<td>Specifies the value that DIAdem uses in the linear mapping process of spike curves for those values to which DIAdem does not assign an interpolation point. The default value of the <span class="Monospace">MapLinInnerVal</span> variable is <span class="Monospace">0</span>.<div id="exp_MapLinInnerVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels with the y-values converted the new x-value range. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.<p class="body">The names of the result channels are composed of <span class="monospace">LinearMapped_</span> and the respective name of the y-channel.</p>
</td></tr>
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
oMyResultChn = dd.ChnMapLinCalcExt(oMyXChannel, oMyChannelList, oMyX1Channel, True, ". value", dd.NoValue, "analogue", 0)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[4]/T*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnMapLinCalcExt("[1]/[1]", oMyChannelList, "[1]/[3]", True, ". value", dd.NoValue, "analogue", 0)
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnMapLinCalcExt.htm`*
