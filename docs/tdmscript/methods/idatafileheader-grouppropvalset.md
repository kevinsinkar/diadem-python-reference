---
title: "IDataFileHeader.GroupPropValSet"
description: "Sets the value of a group property."
---

# IDataFileHeader.GroupPropValSet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropValSet for DataFileHeader

Sets the value of a group property.

## Signature

```python
obj.GroupPropValSet(GroupIndex, PropertyName, PropertyValue)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyDataFileHeader.GroupPropValSet(1,"Description","Test")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropValSet_IDataFileHeader.htm`*
