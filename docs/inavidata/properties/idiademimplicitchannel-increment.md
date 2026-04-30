---
title: "IDiademImplicitChannel.Increment"
description: "Specifies the step width of the values of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.Increment

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Increment for ImplicitChannel <Data>

Specifies the step width of the values of an implicit channel in the script interface for internal data.

## Signature

```python
obj.Increment
```

## Python example

```python
oMyChn = dd.Data.Root.ActiveChannelGroup.Channels(1)
if (oMyChn.IsKindOf(dd.eDataImplicitChannel)) :
    dd.MsgBoxDisp("Channel name: " + oMyChn.Name + "\r\n" + "Increment: " + oMyChn.Increment)
else:
    dd.MsgBoxDisp("No implicit channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Increment_IDiademImplicitChannel.htm`*
