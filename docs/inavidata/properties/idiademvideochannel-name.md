---
title: "IDiademVideoChannel.Name"
description: "Specifies the name of a video channel in the script interface for internal data. The value of the Name for VideoChannel property is the same as the value of Val"
---

# IDiademVideoChannel.Name

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Name for VideoChannel <Data>

Specifies the name of a video channel in the script interface for internal data. The value of the Name for VideoChannel property is the same as the value of Value for Property <Data> with the property value name .

## Signature

```python
obj.Name
```

## Python example

```python
oMyVideoChn= dd.Data.Root.ChannelGroups(1).Channels.AddVideoChannel("Video", "Safetytest02.wmv", dd.eFilePathRelative,dd.NoValue, dd.NoValue, 1)
print(oMyVideoChn.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Name_IDiademVideoChannel.htm`*
