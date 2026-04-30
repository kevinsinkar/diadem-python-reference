---
title: "IDataFileHeader.RootPropDel"
description: "Deletes a root custom property from a TDM header file."
---

# IDataFileHeader.RootPropDel

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropDel for DataFileHeader

Deletes a root custom property from a TDM header file.

## Signature

```python
obj.RootPropDel(PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.RootPropDel("test")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropDel_IDataFileHeader.htm`*
