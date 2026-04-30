---
title: "IDataFileHeader.GroupNameGet"
description: "Determines the name of a group from a TDM header file."
---

# IDataFileHeader.GroupNameGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupNameGet for DataFileHeader

Determines the name of a group from a TDM header file.

## Signature

```python
sGroupNameGet = Object.GroupNameGet(GroupIndex)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupName = oMyDataFileHeader.GroupNameGet(1)
print (oMyGroupName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupNameGet_IDataFileHeader.htm`*
