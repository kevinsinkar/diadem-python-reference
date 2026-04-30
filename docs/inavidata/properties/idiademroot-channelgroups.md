---
title: "IDiademRoot.ChannelGroups"
description: "Contains the ChannelGroups collection associated with a Root object in the script interface for internal data."
---

# IDiademRoot.ChannelGroups

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelGroups for Root <Data>

Contains the ChannelGroups collection associated with a Root object in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelGroups
```

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    oMyProp = oMyChn.Properties
    if oMyProp.Exists("Test_Status") :
        oMyProp("Test_Status").Value = "failed"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelGroups_IDiademRoot.HTM`*
