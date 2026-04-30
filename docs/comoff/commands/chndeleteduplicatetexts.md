---
title: "ChnDeleteDuplicateTexts"
description: "Deletes identical texts from a channel. If you specify more dependent channels in ChnList1 , DIAdem also deletes the respective values in these channels."
---

# ChnDeleteDuplicateTexts

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDeleteDuplicateTexts

Deletes identical texts from a channel. If you specify more dependent channels in ChnList1 , DIAdem also deletes the respective values in these channels.

## Signature

```python
return_value = dd.ChnDeleteDuplicateTexts( Y , ChnList1, [DeleteDuplicateTextsCaseSensitive], [DeleteDuplicatesInPlace], [DeleteDuplicatesMode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values you want to correct. If you specify more dependent channels in <span class="Monospace">ChnList1</span>, DIAdem also deletes the respective values in these channels.</td></tr>
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[DeleteDuplicateTextsCaseSensitive]</td>
<td>Specifies whether text channels in DIAdem are case sensitive.<div id="exp_DeleteDuplicateTextsCaseSensitive">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[DeleteDuplicatesInPlace]</td>
<td>Specifies that DIAdem stores the results in the original channels. DIAdem creates new channels by default.<div id="exp_DeleteDuplicatesInPlace">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[DeleteDuplicatesMode]</td>
<td>Specifies which value DIAdem accepts from the dependent channels.<div id="exp_DeleteDuplicatesMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FirstValue"</pre></donottranslate></td>
<td>First value</td></tr>
<tr><td width="150"><donottranslate><pre>"LastValue"</pre></donottranslate></td>
<td>Last value</td></tr>
<tr><td width="150"><donottranslate><pre>"FirstNonNoValue"</pre></donottranslate></td>
<td>First NoValue value</td></tr>
<tr><td width="150"><donottranslate><pre>"LastNonNoValue"</pre></donottranslate></td>
<td>Last NoValue value</td></tr>
<tr><td width="150"><donottranslate><pre>"Minimum"</pre></donottranslate></td>
<td>Minimum</td></tr>
<tr><td width="150"><donottranslate><pre>"Maximum"</pre></donottranslate></td>
<td>Maximum</td></tr>
<tr><td width="150"><donottranslate><pre>"Mean"</pre></donottranslate></td>
<td>Mean value</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If you select <span class="Monospace">“FirstValue”</span> and the channel you want to cleanse has, for example, the same values from the third to the fifth position, DIAdem deletes the fourth and fifth value of the dependent channels and only retains the third value. If you select <span class="Monospace">"LastValue"</span>, DIAdem in this example deletes the third and fourth value of the dependent channels and only retains the fifth value.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels with the corrected values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyYChannel = dd.Data.Root.ChannelGroups(3).Channels(1)
oMyChannelList = dd.Data.GetChannels("[3]/FirstChnRelated*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnDeleteDuplicateTexts(oMyYChannel, oMyChannelList, False, False, "FirstNonNoValue")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[3]/FirstChnRelated*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnDeleteDuplicateTexts("[3]/[1]", oMyChannelList, False, False, "FirstNonNoValue")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnDeleteDuplicateTexts.htm`*
