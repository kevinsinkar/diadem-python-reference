---
title: "IDataFileHeader.GroupPropValGet"
description: "Determines the value of a group property from a TDM header file."
---

# IDataFileHeader.GroupPropValGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropValGet for DataFileHeader

Determines the value of a group property from a TDM header file.

## Signature

```python
vGroupPropValGet = Object.GroupPropValGet(GroupIndex, PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyGroupPropVal = oMyDataFileHeader.GroupPropValGet(1, "Description")
print (oMyGroupPropVal)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropValGet_IDataFileHeader.htm`*
