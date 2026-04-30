---
title: "DataBlClpPaste"
description: "Pastes a data block from the clipboard into channels. DIAdem moves existing values down."
---

# DataBlClpPaste

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlClpPaste

Pastes a data block from the clipboard into channels. DIAdem moves existing values down.

## Signature

```python
dd.DataBlClpPaste(ChnList, ChnRow, [ValNo], [ValOnly])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../../../inavidata/methods/idiademchannel-getvaluesblock/">GetValuesBlock</a> and <a href="../../../inavidata/methods/idiademchannel-setvaluesblock/">SetValuesBlock</a> methods instead.<p class="Body">If you assign the value <span class="Monospace">0</span> to the <span class="Monospace">ValNo</span> variable or if you do not specify the <span class="Monospace">ValNo</span> parameter, DIAdem pastes all values from the clipboard.</p>
<p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="Body">The <span class="Monospace">DataBlClpPaste</span> command replaces the <a href="../dataareaclppaste/">DataAreaClpPaste</a> command.</p>
</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ChnRow</td>
<td>Specifies the row number in a channel.<div id="exp_ChnRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ChnRow &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ValNo]</td>
<td>Specifies the number of values in a channel.<div id="exp_ValNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ValNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ValOnly]</td>
<td>Specifies whether DIAdem should overwrite the channel names, the description, and the unit, when the target channel is length zero and the clipboard contains the channel name, the description, and the unit. For example, the <a href="../datablclpcopy/">DataBlClpCopy</a> command copies the channel name and the unit to the clipboard. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem overwrites the properties.<div id="exp_ValOnly">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[3]/Res_Noise*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.DataBlClpCopy(oMyChannelList, 1, 4)
dd.DataBlClpPaste(oMyChannelList, 5)
```

---

*Source: `ComOff/DataBlClpPaste.htm`*
