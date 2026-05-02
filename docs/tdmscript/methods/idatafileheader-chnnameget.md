---
title: "IDataFileHeader.ChnNameGet"
description: "Determines the name of a channel from a TDM header file."
---

# IDataFileHeader.ChnNameGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnNameGet for DataFileHeader

Determines the name of a channel from a TDM header file.

## Signature

```python
sChnNameGet = Object.ChnNameGet(GroupIndex, TargetChnIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyChnName = oMyDataFileHeader.ChnNameGet(1,2)
print (oMyChnName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnNameGet_IDataFileHeader.htm`*
