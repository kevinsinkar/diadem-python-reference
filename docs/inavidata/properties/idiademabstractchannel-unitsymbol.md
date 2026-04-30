---
title: "IDiademAbstractChannel.UnitSymbol"
description: "Specifies the unit symbol of a channel."
---

# IDiademAbstractChannel.UnitSymbol

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: UnitSymbol for BaseChannel <Data>

Specifies the unit symbol of a channel.

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
dd.MsgBoxDisp(oMyChannel.UnitSymbol) # equivalent to oMyChannel.Properties("unit_string").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_UnitSymbol_IDiademAbstractChannel.htm`*
