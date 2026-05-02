---
title: "IDataFileHeader.FileName"
description: "Specifies the name of a TDM header file."
---

# IDataFileHeader.FileName

!!! abstract "Property &middot; `TDMScript.chm`"
    Property: FileName for DataFileHeader

Specifies the name of a TDM header file.

## Signature

```python
obj.FileName
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyChnName = oMyDataFileHeader.ChnNameGet(1,2)
print(oMyDataFileHeader.FileName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/properties/TDM_property_FileName_IDataFileHeader.htm`*
