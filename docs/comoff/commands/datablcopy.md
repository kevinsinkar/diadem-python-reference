---
title: "DataBlCopy"
description: "Copies a data block from channels and inserts the data block into other channels. DIAdem overwrites existing values."
---

# DataBlCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlCopy

Copies a data block from channels and inserts the data block into other channels. DIAdem overwrites existing values.

## Signature

```python
dd.DataBlCopy(ChnList, ChnRow, ValNo, ChnList1, TargetLine)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong><p class="Body">The <span class="Monospace">DataBlCopy</span> command replaces the <a href="../dataareacopy/">DataAreaCopy</a> command.</p>
<p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="Body">The number of source and target channels must be identical.</p>
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
dd.DataBlCopy(oMyChannelList1, 3, 10, oMyChannelList2, 2)
```

---

*Source: `ComOff/DataBlCopy.htm`*
