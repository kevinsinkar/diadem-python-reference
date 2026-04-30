---
title: "IDiademComplexChannel.Minimum"
description: "Specifies the minimum value of a complex channel . The value of the Minimum property for ComplexChannel corresponds to the value of Object .Properties(\"minimum\""
---

# IDiademComplexChannel.Minimum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Minimum for ComplexChannel <Data>

Specifies the minimum value of a complex channel . The value of the Minimum property for ComplexChannel corresponds to the value of Object .Properties("minimum").value .

## Signature

```python
obj.Minimum
```

## Python example

```python
oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
dd.MsgBoxDisp(oMyChannel.Minimum) # is equivalent to oMyChannel.Properties("minimum").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Minimum_IDiademComplexChannel.htm`*
