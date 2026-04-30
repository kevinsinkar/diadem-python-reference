---
title: "IDiademChannel.Properties"
description: "Contains the Properties collection that is associated with a ChannelGroup object in the script interface for internal data."
---

# IDiademChannel.Properties

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Properties for Channel <Data>

Contains the Properties collection that is associated with a ChannelGroup object in the script interface for internal data.

## Signature

```python
return_value = obj.Properties
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> for information about properties of files, groups, and channels.</td></tr></table>
</div>

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    if oMyChn.Properties.Exists("Sensor_Type") :
        bFound = True
    else:
        oMyChn.Properties.Add("Sensor_Type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Properties_IDiademChannel.HTM`*
