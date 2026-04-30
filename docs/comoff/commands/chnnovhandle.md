---
title: "ChnNovHandle"
description: "Removes or interpolates NoValues in data channels."
---

# ChnNovHandle

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNovHandle

Removes or interpolates NoValues in data channels.

## Signature

```python
dd.ChnNovHandle(CALCXChn, CALCYChn, NovMeth, NovCtrlChn, [ChnNovIP], NoVChnX, [NovReplaceVal])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td class="style1"><strong>Note</strong>  If you want to edit a waveform channel, select <span class="Monospace">NoVChnX = True</span> and enter the waveform channel as x-channel. If the y-share of the waveform channel is not monotonic increasing, you can only delete or replace but not interpolate NoValues in this channel. If you want to process several waveform channels, you must generate a matching x-channel with the <a href="#" data-unresolved="1">Numeric Channels &lt;-&gt; Waveform Channels</a> function.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To interpolate NoValues, the values in the x-channel must be monotonic increasing.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the data channels you want to process do not contain NoValues, DIAdem does not create a result channel.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If DIAdem deletes NoValues in a data channel, the succeeding values move up. The result channel becomes shorter. If the input channels only contain NoValues, DIAdem generates empty result channels.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not overwrite the result channels, DIAdem saves the result channels in the default group.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CALCXChn</td>
<td>Specifies the data channel containing the x-values of the signal.<div id="exp_CALCXChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CALCYChn</td>
<td>Specifies the data channels containing the y-values of the signal.<div id="exp_CALCYChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">NovMeth</td>
<td>Specifies whether DIAdem replaces <a href="../../../varoff/variables/nv/">NoValues</a> with linearly-interpolated or specified values, or whether DIAdem deletes NoValues.<div id="exp_NovMeth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Delete"</pre></donottranslate></td>
<td>Delete</td></tr>
<tr><td width="150"><donottranslate><pre>"Interpolate"</pre></donottranslate></td>
<td>Interpolate</td></tr>
<tr><td width="150"><donottranslate><pre>"SetValue"</pre></donottranslate></td>
<td>Replace</td></tr>
</table>
</td></tr>
</table>
<p class="Body"><strong>Valid settings</strong></p>
<table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" height="33" id="AutoNumber1" style="border-collapse: collapse">
<tr>
<td height="20" width="150"><span class="Monospace">Delete</span></td>
<td height="20">You can specify whether DIAdem deletes all NoValues in the x-channel and the corresponding values in the y-channels or whether DIAdem inspects the specified channels and deletes all NoValues and the corresponding values of the other channels channel by channel.</td>
</tr>
<tr>
<td height="13" width="150"><span class="Monospace">Interpolate</span></td>
<td height="13">DIAdem replaces the NoValues found in x-channels by equidistant values between the adjacent valid numbers. DIAdem replaces the NoValues found in y-channels by linearly interpolated values, which the program calculates based on the x-channel.</td>
</tr>
<tr>
<td height="13" width="150"><span class="Monospace">SetValue</span></td>
<td height="13">DIAdem replaces NoValues in the channels with the value <a href="../../../varoff/variables/novreplaceval/">NovReplaceVal</a>.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">NovCtrlChn</td>
<td>Specifies whether DIAdem searches for <a href="../../../varoff/variables/nv/">NoValues</a> only in the x-channel or also in the y-channels.<div id="exp_NovCtrlChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"X"</pre></donottranslate></td>
<td>Only x-channel</td></tr>
<tr><td width="150"><donottranslate><pre>"XY"</pre></donottranslate></td>
<td>X-channels and y-channels</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If you assign the value <span class="Monospace">X</span> to the variable <span class="Monospace">NovCtrlChn</span>, DIAdem deletes all NoValues in the x-channel and the corresponding values in the y-channels. If you assign the value <span class="Monospace">XY</span> to the variable <span class="Monospace">NovCtrlChn</span>, DIAdem inspects all specified channels and deletes all NoValues and the corresponding values of the other channels channel by channel.</p>
</div></td></tr>
<tr><td width="150">[ChnNovIP]</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result channels of NoValue processing. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not overwrite the input channels.<div id="exp_ChnNovIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">NoVChnX</td>
<td>Specifies whether DIAdem processes one data channel or several. If the value is <span class="Monospace">TRUE</span>, DIAdem processes only one channel.<div id="exp_NoVChnX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[NovReplaceVal]</td>
<td>Specifies the value with which DIAdem replaces <a href="#" data-unresolved="1">NoValues</a>. The default value of the <span class="Monospace">NovReplaceVal</span> variable is <span class="Monospace">0</span>.<div id="exp_NovReplaceVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ChnNovHandle("Group/Channel1","Group/Channel2","Delete","X",False,False)
```

---

*Source: `ComOff/ChnNovHandle.htm`*
