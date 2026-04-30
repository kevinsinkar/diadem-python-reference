---
title: "IDiademImplicitChannel.Maximum"
description: "Specifies the maximum of an implicit channel. The value of the Maximum property for ImplicitChannel corresponds to the value of Object .Properties(\"maximum\").va"
---

# IDiademImplicitChannel.Maximum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Maximum for ImplicitChannel <Data>

Specifies the maximum of an implicit channel. The value of the Maximum property for ImplicitChannel corresponds to the value of Object .Properties("maximum").value .

## Signature

```python
obj.Maximum
```

## Python example

```python
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
dd.MsgBoxDisp(oMyImplChannel.Maximum) # equivalent to oMyImplChannel.Properties("maximum").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Maximum_IDiademImplicitChannel.htm`*
