---
title: "DataBlInsert"
description: "Copies a data block from channels and inserts the data block into other channels. In the process DIAdem moves existing values down."
---

# DataBlInsert

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlInsert

Copies a data block from channels and inserts the data block into other channels. In the process DIAdem moves existing values down.

## Signature

```python
dd.DataBlInsert(ChnList, ChnRow, ValNo, ChnList1, TargetLine)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong><p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="Body">The number of source and target channels must be identical.</p>
<p class="Body">You cannot perform block operations on text channels.</p>
<p class="Body">If you want to copay a data block from the end of a channel to the beginning of that channel, DIAdem does not copy the data as expected. In this case, instead of using the <span class="Monospace">DataBlInsert</span> command, use the methods <a href="../../../inavidata/methods/idiademchannel-setvaluesblock/">SetValuesBlock</a> and <a href="../../../inavidata/methods/idiademchannel-getvaluesblock/">GetValuesBlock</a>.</p>
<p class="body">The <span class="Monospace">DataBlInsert</span> command replaces the <a href="../dataareainsert/">DataAreaInsert</a> command.</p>
</td>
</tr>
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
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">TargetLine</td>
<td>Specifies the row number in the target channel.<div id="exp_TargetLine">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= TargetLine &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList1 = dd.Data.GetChannels("[1]/Channel1")
oMyChannelList1.Add(dd.Data.Root.ChannelGroups(1).Channels("Channel2"))
oMyChannelList2 = dd.Data.GetChannels("[2]/[1]")
oMyChannelList2.Add(dd.Data.Root.ChannelGroups(2).Channels(2))
dd.DataBlInsert(oMyChannelList1, 3, 10, oMyChannelList2, 2)
```

---

*Source: `ComOff/DataBlInsert.htm`*
