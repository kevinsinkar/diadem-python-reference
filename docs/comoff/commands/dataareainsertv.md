---
title: "DataAreaInsertV"
description: "Inserts a data block with values into channels. In the process DIAdem moves existing values down."
---

# DataAreaInsertV

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataAreaInsertV

Inserts a data block with values into channels. In the process DIAdem moves existing values down.

## Signature

```python
dd.DataAreaInsertV(ChnArg1, ChnRow, ValNo, ChnArg2, [ValueInsert])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note</strong><p class="body">The <a href="../datablinsertval/">DataBlInsertVal</a> command replaces the <span class="Monospace">DataAreaInsertV</span> command.</p>
<p class="Body">The channels used are in the same order as the channel numbers. This order is not always the same as the order of the channels in the Data Portal.</p>
<p class="Body">You cannot perform block operations on text channels.</p>
</td></tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnArg1</td>
<td>Specifies a channel.<div id="exp_ChnArg1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to clearly specify channels.</p>
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
<tr><td width="150">ChnArg2</td>
<td>Specifies a further channel.<div id="exp_ChnArg2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to specify channels.</p>
</div></td></tr>
<tr><td width="150">[ValueInsert]</td>
<td>Specifies the value that DIAdem inserts. The default value of the <span class="Monospace">ValueInsert</span> variable is <span class="Monospace">0</span>.<div id="exp_ValueInsert">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DataAreaInsertV("Group1/Channel1",1,10,"Group1/Channel4",1)
```

---

*Source: `ComOff/DataAreaInsertV.htm`*
