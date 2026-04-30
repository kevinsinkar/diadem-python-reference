---
title: "IDiademImplicitChannel.ValueIndex"
description: "Determines the row in an implicit channel with contents closest to a given value."
---

# IDiademImplicitChannel.ValueIndex

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ValueIndex for ImplicitChannel <Data>

Determines the row in an implicit channel with contents closest to a given value.

## Signature

```python
obj.ValueIndex(ValueToSearch)
```

## Python example

```python
oMyChn = dd.Data.Root.ChannelGroups("Group1").Channels("Input")
intMyResult = oMyChn.ValueIndex(77)
```

---

*Source: `Inavidata/properties/DiaCmpnt_property_ValueIndex_IDiademImplicitChannel.htm`*
