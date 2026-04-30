---
title: "ChnFlagDel"
description: "Deletes all the Flags of a channel."
---

# ChnFlagDel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFlagDel

Deletes all the Flags of a channel.

## Signature

```python
dd.ChnFlagDel( X )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../../../inavidata/properties/idiademchannel-operationalflags/">OperationalFlags</a> property to assign a flag to a channel value. Use the <a href="../chnflagdelall/">ChnFlagDelAll</a> command to delete all flags of all channels. Use the <a href="../chnflagset/">ChnFlagSet</a> command to set or to delete several flags in a channel.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnFlagDel("Group1/Channel1")
```

---

*Source: `ComOff/ChnFlagDel.htm`*
