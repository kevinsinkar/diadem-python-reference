---
title: "IDiademImplicitChannel.Minimum"
description: "Specifies the minimum value of an implicit channel. The value of the Minimum property for ImplicitChannel corresponds to the value of Object .Properties(\"minimu"
---

# IDiademImplicitChannel.Minimum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Minimum for ImplicitChannel <Data>

Specifies the minimum value of an implicit channel. The value of the Minimum property for ImplicitChannel corresponds to the value of Object .Properties("minimum").value .

## Signature

```python
obj.Minimum
```

## Python example

```python
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
dd.MsgBoxDisp(oMyImplChannel.Minimum) # equivalent to oMyImplChannel.Properties("minimum").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Minimum_IDiademImplicitChannel.htm`*
