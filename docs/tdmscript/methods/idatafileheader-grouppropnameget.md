---
title: "IDataFileHeader.GroupPropNameGet"
description: "Determines the name of a group property from a TDM header file."
---

# IDataFileHeader.GroupPropNameGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropNameGet for DataFileHeader

Determines the name of a group property from a TDM header file.

## Signature

```python
sGroupPropNameGet = Object.GroupPropNameGet(GroupIndex, GroupPropIndex)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupPropName = oMyDataFileHeader.GroupPropNameGet(1,2)
print (oMyGroupPropName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropNameGet_IDataFileHeader.htm`*
