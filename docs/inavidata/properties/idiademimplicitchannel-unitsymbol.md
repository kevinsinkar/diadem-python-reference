---
title: "IDiademImplicitChannel.UnitSymbol"
description: "Specifies the unit symbol of an implicit channel. The value of the UnitSymbol property for Implicit Channel corresponds to the value of Object .Properties(\"unit"
---

# IDiademImplicitChannel.UnitSymbol

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: UnitSymbol for ImplicitChannel <Data>

Specifies the unit symbol of an implicit channel. The value of the UnitSymbol property for Implicit Channel corresponds to the value of Object .Properties("unit_string").value .

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
dd.MsgBoxDisp(oMyImplChannel.UnitSymbol) # equivalent to oMyImplChannel.Properties("unit_string").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_UnitSymbol_IDiademImplicitChannel.htm`*
