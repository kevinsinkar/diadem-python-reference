---
title: "IDataFileHeader.RootPropNameGet"
description: "Determines the name of a data set property from a TDM header file."
---

# IDataFileHeader.RootPropNameGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropNameGet for DataFileHeader

Determines the name of a data set property from a TDM header file.

## Signature

```python
sRootPropNameGet = Object.RootPropNameGet(RootPropIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyRootPropName = oMyDataFileHeader.RootPropNameGet(2)
print (oMyRootPropName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropNameGet_IDataFileHeader.htm`*
