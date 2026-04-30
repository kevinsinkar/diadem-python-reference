---
title: "DataBlAppend"
description: "Copies data blocks from channels and appends the data blocks to other channels."
---

# DataBlAppend

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlAppend

Copies data blocks from channels and appends the data blocks to other channels.

## Signature

```python
dd.DataBlAppend(ChnList, ChnRow, ValNo, ChnList1)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong><p class="Body">The <span class="Monospace">DataBlAppend</span> command replaces the <a href="../dataareaappend/">DataAreaAppend</a> command.</p>
<p class="Body">The order of the channels you use is not the same as the displayed order in the Data Portal.</p>
<p class="Body">To determine the number of the row where DIAdem inserts the copied data block, DIAdem determines which row in the target channels has the last valid value. If the channels are not the same length, the result channel might have gaps.</p>
<p class="Body">Source and target channels must not be identical. The number of source and target channels must be identical.</p>
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
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList1 = dd.Data.GetChannels("[1]/Channel1")
oMyChannelList1.Add(dd.Data.Root.ChannelGroups(1).Channels("Channel2"))
oMyChannelList2 = dd.Data.GetChannels("[2]/[1]")
oMyChannelList2.Add(dd.Data.Root.ChannelGroups(2).Channels(2))
dd.DataBlAppend(oMyChannelList1,3,10,oMyChannelList2)
```

---

*Source: `ComOff/DataBlAppend.htm`*
