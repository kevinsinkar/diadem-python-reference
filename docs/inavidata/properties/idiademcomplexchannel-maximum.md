---
title: "IDiademComplexChannel.Maximum"
description: "Specifies the maximum value of a complex channel . The value of the Maximum property for ComplexChannel corresponds to the value of Object .Properties(\"maximum\""
---

# IDiademComplexChannel.Maximum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Maximum for ComplexChannel <Data>

Specifies the maximum value of a complex channel . The value of the Maximum property for ComplexChannel corresponds to the value of Object .Properties("maximum").value .

## Signature

```python
obj.Maximum
```

## Python example

```python
oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
dd.MsgBoxDisp(oMyChannel.Maximum) #equivalent to oMyChannel.Properties("maximum").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Maximum_IDiademComplexChannel.htm`*
