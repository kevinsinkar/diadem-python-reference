---
title: "ChnPropCopy"
description: "Copies all channel properties to another channel. You also can use the object-oriented interface to access internal data. Use the AddProperties for Properties t"
---

# ChnPropCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPropCopy

Copies all channel properties to another channel. You also can use the object-oriented interface to access internal data. Use the AddProperties for Properties to implement the functionality of the ChnPropCopy command with the script interface for internal data.

## Signature

```python
dd.ChnPropCopy(SourceChn, TargetChn)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">ChnPropCopy</span> command does not copy the channel name, calculated properties, and management properties.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SourceChn</td>
<td>Specifies the input channel.<div id="exp_SourceChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to specify channels.</p>
</div></td></tr>
<tr><td width="150">TargetChn</td>
<td>Specifies the target channel.<div id="exp_TargetChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to specify channels.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnPropCopy.htm`*
