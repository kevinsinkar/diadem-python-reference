---
title: "IDiademImplicitChannel.Properties"
description: "Returns the properties of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.Properties

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Properties for ImplicitChannel <Data>

Returns the properties of an implicit channel in the script interface for internal data.

## Signature

```python
return_value = obj.Properties
```

## Python example

```python
oMyChn = dd.Data.Root.ActiveChannelGroup.Channels(1)
if oMyChn.Properties.Exists("TimeBegin") :
    oMyChn.Properties.Add("TimeEnd", dd.CurrTime)
else:
    dd.MsgBoxDisp("Property TimeBegin does not exist")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Properties_IDiademImplicitChannel.htm`*
