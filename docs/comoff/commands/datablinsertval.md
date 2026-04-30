---
title: "DataBlInsertVal"
description: "Inserts a data block, in which all the values are the same, into channels. DIAdem moves existing values down."
---

# DataBlInsertVal

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataBlInsertVal

Inserts a data block, in which all the values are the same, into channels. DIAdem moves existing values down.

## Signature

```python
dd.DataBlInsertVal(ChnList, ChnRow, ValNo, [ValueInsert], [ValueOverwrite])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong><p class="Body">The order of the channels you use is not always the same as the displayed order in the Data Portal.</p>
<p class="Body">The <span class="Monospace">DataBlInsertVal</span> command replaces the <a href="../dataareainsertv/">DataAreaInsertV</a> command.</p>
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
<tr><td width="150">[ValueInsert]</td>
<td>Specifies the value that DIAdem inserts. The default value of the <span class="Monospace">ValueInsert</span> variable is <span class="Monospace">0</span>.<div id="exp_ValueInsert">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ValueOverwrite]</td>
<td>Specifies whether DIAdem overwrites existing channel data. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not overwrite the input channels.<div id="exp_ValueOverwrite">
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
dd.DataBlInsertVal(oMyChannelList, 4, 10, 9, False)
```

---

*Source: `ComOff/DataBlInsertVal.htm`*
