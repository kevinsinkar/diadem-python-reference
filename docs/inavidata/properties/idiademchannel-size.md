---
title: "IDiademChannel.Size"
description: "Returns the number of values currently used for a channel, in the script interface for internal data. DIAdem automatically adjusts the value of the Size propert"
---

# IDiademChannel.Size

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Size for Channel <Data>

Returns the number of values currently used for a channel, in the script interface for internal data. DIAdem automatically adjusts the value of the Size property if you write more values to the channel.

## Signature

```python
obj.Size
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You also can use the channel property <a href="#" data-unresolved="1">length</a> to read and write the value of the <span class="Monospace">Size</span> property.</td></tr></table>
</div>

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    dd.MsgBoxDisp (oMyChn.Name + ": " + oMyChn.Size)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Size_IDiademChannel.HTM`*
