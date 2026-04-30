---
title: "IDataFileHeader.GroupPropDel"
description: "Deletes a group custom property from a TDM header file."
---

# IDataFileHeader.GroupPropDel

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropDel for DataFileHeader

Deletes a group custom property from a TDM header file.

## Signature

```python
obj.GroupPropDel(GroupIndex, PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.GroupPropDel(1,"Test1")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropDel_IDataFileHeader.htm`*
