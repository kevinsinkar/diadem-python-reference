---
title: "IDiademChannelGroup.Name"
description: "Receives the name of a ChannelGroup object in the script interface for internal data."
---

# IDiademChannelGroup.Name

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Name for ChannelGroup <Data>

Receives the name of a ChannelGroup object in the script interface for internal data.

## Signature

```python
obj.Name
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The name must conform to the DIAdem conventions. If the name does not conform to the <a href="#" data-unresolved="1">name conventions</a>, DIAdem corrects the name.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.ChannelGroups(1).Name = "Temp"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Name_IDiademChannelGroup.HTM`*
