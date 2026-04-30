---
title: "IDataFileHeader.GroupPropIsFixed"
description: "Determines whether a group property is a TDM property or a custom property."
---

# IDataFileHeader.GroupPropIsFixed

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropIsFixed for DataFileHeader

Determines whether a group property is a TDM property or a custom property.

## Signature

```python
bGroupPropIsFixed = Object.GroupPropIsFixed(GroupIndex, PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.GroupPropIsFixed(1,"maximum") :
    print ("TDM Property")
else:
    print ("Custom Property")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropIsFixed_IDataFileHeader.htm`*
