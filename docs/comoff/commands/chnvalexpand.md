---
title: "ChnValExpand"
description: "Expands registered or implicit channels into standard DIAdem channels."
---

# ChnValExpand

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnValExpand

Expands registered or implicit channels into standard DIAdem channels.

## Signature

```python
dd.ChnValExpand(ChnList)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you previously assigned a channel you expanded with the command <span class="Monospace">ChnValExpand()</span> to an object, you must reassign this channel to the object because you cannot convert an implicit or registered channel object into an explicit channel object. If you do not execute this assignment after the expansion again, the channel object retains the contents it had before the expansion.</td></tr></table>
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
</table>
</div>

---

*Source: `ComOff/ChnValExpand.htm`*
