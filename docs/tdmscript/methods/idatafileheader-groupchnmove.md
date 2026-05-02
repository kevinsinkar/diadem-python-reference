---
title: "IDataFileHeader.GroupChnMove"
description: "Moves a channel to a new position inside a group, in a TDM header file."
---

# IDataFileHeader.GroupChnMove

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupChnMove for DataFileHeader

Moves a channel to a new position inside a group, in a TDM header file.

## Signature

```python
obj.GroupChnMove(SourceChn, TargetChnIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.GroupChnMove("2/1",3)
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupChnMove_IDataFileHeader.htm`*
