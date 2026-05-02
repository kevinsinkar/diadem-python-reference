---
title: "IDataFileHeader.GroupCount"
description: "Determines from a TDM header file the number of groups."
---

# IDataFileHeader.GroupCount

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupCount for DataFileHeader

Determines from a TDM header file the number of groups.

## Signature

```python
iGroupCount = Object.GroupCount
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupCount = oMyDataFileHeader.GroupCount
print (oMyGroupCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupCount_IDataFileHeader.htm`*
