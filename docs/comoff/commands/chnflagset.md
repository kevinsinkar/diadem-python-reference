---
title: "ChnFlagSet"
description: "Sets Flags for several successive values of a channel."
---

# ChnFlagSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFlagSet

Sets Flags for several successive values of a channel.

## Signature

```python
dd.ChnFlagSet(ChnArg1, ChnRow, ValNo, ChnBool )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../../../inavidata/properties/idiademchannel-operationalflags/">OperationalFlags</a> property to assign a flag to a channel value. Use the <a href="../chnflagdelall/">ChnFlagDelAll</a> command to delete all flags of all channels. Use the <a href="../chnflagdel/">ChnFlagDel</a> command to delete all flags of one channel.</td></tr></table>
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
<tr><td width="150">ChnBool</td>
<td>Specifies whether DIAdem sets (<span class="Monospace">TRUE</span>) or deletes (<span class="Monospace">FALSE</span>) <a href="#" data-unresolved="1">Flags</a>.<div id="exp_ChnBool">
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
dd.ChnFlagSet("Group1/Channel1", 5, 10, True)
```

---

*Source: `ComOff/ChnFlagSet.htm`*
