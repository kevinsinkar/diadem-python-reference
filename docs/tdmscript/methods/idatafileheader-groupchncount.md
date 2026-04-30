---
title: "IDataFileHeader.GroupChnCount"
description: "Determines from a TDM header file the number of channels in a group."
---

# IDataFileHeader.GroupChnCount

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupChnCount for DataFileHeader

Determines from a TDM header file the number of channels in a group.

## Signature

```python
iGroupChnCount = Object.GroupChnCount(GroupIndex)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyGroupChnCount = oMyDataFileHeader.GroupChnCount(1)
print (oMyGroupChnCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupChnCount_IDataFileHeader.htm`*
