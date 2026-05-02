---
title: "IDataFileHeader.RootPropValGet"
description: "Determines the value of a data set property from a TDM header file."
---

# IDataFileHeader.RootPropValGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropValGet for DataFileHeader

Determines the value of a data set property from a TDM header file.

## Signature

```python
vRootPropValGet = Object.RootPropValGet(PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyRootPropVal = oMyDataFileHeader.RootPropValGet("Description")
print (oMyRootPropVal)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropValGet_IDataFileHeader.htm`*
