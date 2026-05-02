---
title: "IDataFileHeader.GroupMove"
description: "Moves a group in a TDM header file to a new position."
---

# IDataFileHeader.GroupMove

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupMove for DataFileHeader

Moves a group in a TDM header file to a new position.

## Signature

```python
obj.GroupMove(SourceGroupIndex, TargetGroupIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.GroupMove(1,2)
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupMove_IDataFileHeader.htm`*
