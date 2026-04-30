---
title: "ChnConvertChannelType"
description: "Converts a numeric channel to a complex channel and vice versa. The channel values remain unchanged."
---

# ChnConvertChannelType

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertChannelType

Converts a numeric channel to a complex channel and vice versa. The channel values remain unchanged.

## Signature

```python
return_value = dd.ChnConvertChannelType( Y , ChnTargetType )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong> Complex channels are a preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the channel you want to convert. The input channel may not be write-protected. When converting to a complex channel, this channel must have an even number of values and can be a numeric, waveform, or xy-channel.</td></tr>
<tr><td width="150">ChnTargetType</td>
<td>Specifies the type of the result channel.<div id="exp_ChnTargetType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"numeric"</pre></donottranslate></td>
<td>Numeric channel</td></tr>
<tr><td width="150"><donottranslate><pre>"complex"</pre></donottranslate></td>
<td>Complex channel</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. The result channel overwrites the input channel, but does not modify any channel values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertChannelType.htm`*
