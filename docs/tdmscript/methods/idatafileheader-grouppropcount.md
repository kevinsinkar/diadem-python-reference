---
title: "IDataFileHeader.GroupPropCount"
description: "Determines the number of all group properties of a TDM header file."
---

# IDataFileHeader.GroupPropCount

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropCount for DataFileHeader

Determines the number of all group properties of a TDM header file.

## Signature

```python
iGroupPropCount = Object.GroupPropCount(GroupIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupPropCount = oMyDataFileHeader.GroupPropCount(1)
print (oMyGroupPropCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropCount_IDataFileHeader.htm`*
