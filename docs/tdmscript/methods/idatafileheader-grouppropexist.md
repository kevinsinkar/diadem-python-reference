---
title: "IDataFileHeader.GroupPropExist"
description: "Determines whether a group property exists."
---

# IDataFileHeader.GroupPropExist

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupPropExist for DataFileHeader

Determines whether a group property exists.

## Signature

```python
bGroupPropExist = Object.GroupPropExist(GroupIndex, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.GroupPropExist(1,"Test") :
    print ("Exists")
else:
    print() ("Doesn't exist")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupPropExist_IDataFileHeader.htm`*
