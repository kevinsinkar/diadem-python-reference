---
title: "DataBlClpCopy"
description: "Copies a data block from channels into the clipboard."
---

# DataBlClpCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlClpCopy

Copies a data block from channels into the clipboard.

## Signature

```python
dd.DataBlClpCopy(ChnList, ChnRow, ValNo)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong><p class="body">Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../../../inavidata/methods/idiademchannel-getvaluesblock/">GetValuesBlock</a> and <a href="../../../inavidata/methods/idiademchannel-setvaluesblock/">SetValuesBlock</a> methods instead.</p>
<p class="Body">The <span class="Monospace">DataBlClpCopy</span> command replaces the <a href="../dataareaclpcopy/">DataAreaClpCopy</a> command.</p>
<p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="body">In the clipboard, tabulators separate data blocks that are from different channels.</p>
</td></tr>
</table>
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
<tr><td width="150">ValNo</td>
<td>Specifies the number of values in a channel.<div id="exp_ValNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ValNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.DataBlClpCopy(oMyChannelList, 4, 10)
```

---

*Source: `ComOff/DataBlClpCopy.htm`*
