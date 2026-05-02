---
title: "IDataFileHeader.GroupPropDataTypeGet"
description: "Determines the data type of a group property of a TDM header file."
---

# IDataFileHeader.GroupPropDataTypeGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropDataTypeGet for DataFileHeader

Determines the data type of a group property of a TDM header file.

## Signature

```python
iGroupPropDataTypeGet = Object.GroupPropDataTypeGet(GroupIndex, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupPropDataType = oMyDataFileHeader.GroupPropDataTypeGet(1,"Description")
print (oMyGroupPropDataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropDataTypeGet_IDataFileHeader.htm`*
