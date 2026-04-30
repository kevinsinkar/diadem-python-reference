---
title: "IDiademChannel.ReservedSize"
description: "Specifies the number of values that DIAdem reserves for a channel, in the script interface for internal data. DIAdem automatically adjusts the value of the Rese"
---

# IDiademChannel.ReservedSize

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ReservedSize for Channel <Data>

Specifies the number of values that DIAdem reserves for a channel, in the script interface for internal data. DIAdem automatically adjusts the value of the ReservedSize property if a channel requires more values than specified.

## Signature

```python
obj.ReservedSize
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can also use the <a href="#" data-unresolved="1">lengthmax</a> channel property to determine the value of the <span class="Monospace">ReservedSize</span> property.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you set the value for the <span class="Monospace">ReservedSize</span> property, you cannot decrease this value again.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.Data.Root.ChannelGroups(1).Channels(1).ReservedSize)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ReservedSize_IDiademChannel.HTM`*
