---
title: "ChnConcat"
description: "Possible spellings: ChnConcat, ChnConcatenate"
---

# ChnConcat

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConcat

Possible spellings: ChnConcat, ChnConcatenate

## Signature

```python
dd.ChnConcat(ChnArg1, ChnArg2)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can append channels to channels that have the same data type.</td></tr></table>
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
<p class="Body">A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to clearly specify channels.</p>
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
</table>
</div>

## Python example

```python
dd.ChnConcat("Group/SourceChannel","Group/TargetChannel")
```

---

*Source: `ComOff/ChnConcat.htm`*
