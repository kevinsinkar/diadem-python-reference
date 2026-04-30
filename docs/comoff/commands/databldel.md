---
title: "DataBlDel"
description: "Deletes a data block in channels."
---

# DataBlDel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlDel

Deletes a data block in channels.

## Signature

```python
dd.DataBlDel(ChnList, ChnRow, ValNo, [ValDelOnly])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong><p class="Body">The <span class="Monospace">DataBlDel</span> command replaces the <a href="../dataareadel/">DataAreaDel</a> command.</p>
<p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="Body">If you delete data blocks in a channel, DIAdem moves up the subsequent data in the channel.</p>
<p class="Body">You cannot perform block operations on text channels.</p>
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
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
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
<tr><td width="150">[ValDelOnly]</td>
<td>Specifies whether DIAdem deletes only the channel values or also all properties when deleting all values. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem also deletes the properties.<div id="exp_ValDelOnly">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.DataBlDel(oMyChannelList, 4, 10)
```

---

*Source: `ComOff/DataBlDel.htm`*
