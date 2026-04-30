---
title: "ChannelsToArray"
description: "Possible spellings: ChannelsToArray, ChnToValue, ChnToVariant"
---

# ChannelsToArray

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChannelsToArray

Possible spellings: ChannelsToArray, ChnToValue, ChnToVariant

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Use the ChannelsToArray syntax instead of ChnToValue or ChnToVariant.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[ForceVariantType]</td>
<td>Specifies whether DIAdem transposes the array with the channel data. DIAdem does not transpose this array by default.<div id="exp_ForceVariantType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Matrix"</pre></donottranslate></td>
<td>Matrix</td></tr>
<tr><td width="150"><donottranslate><pre>"TransposedMatrix"</pre></donottranslate></td>
<td>Transposed matrix</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type.</td></tr>
</table>
</div>

## Python example

```python
MyArray = dd.ChannelsToArray("[1]/[1]")
print(len(MyArray))
```

---

*Source: `ComOff/ChannelsToArray.htm`*
