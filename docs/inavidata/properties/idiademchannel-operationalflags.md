---
title: "IDiademChannel.OperationalFlags"
description: "Specifies whether DIAdem assigns a flag to the value of a channel in the script interface for internal data."
---

# IDiademChannel.OperationalFlags

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: OperationalFlags for Channel <Data>

Specifies whether DIAdem assigns a flag to the value of a channel in the script interface for internal data.

## Signature

```python
obj.OperationalFlags(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To delete all flags of all the channels, use the <a href="../../../comoff/commands/chnflagdelall/">ChnFlagDelAll</a> command. To delete the flags of one channel, use the <a href="../../../comoff/commands/chnflagdel/">ChnFlagDel</a> command. To delete or to set several flags in one channel, use the <a href="../../../comoff/commands/chnflagset/">ChnFlagSet</a> command.</td></tr></table>
</div>

## Python example

```python
oMyDataChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
oMyDataChannel.OperationalFlags[1] = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_OperationalFlags_IDiademChannel.htm`*
