---
title: "IDataFileHeader.GroupSwap"
description: "Swaps two groups in a TDM header file."
---

# IDataFileHeader.GroupSwap

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: GroupSwap for DataFileHeader

Swaps two groups in a TDM header file.

## Signature

```python
obj.GroupSwap(SourceGroupIndex, TargetGroupIndex)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.GroupSwap(1,2)
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_GroupSwap_IDataFileHeader.htm`*
