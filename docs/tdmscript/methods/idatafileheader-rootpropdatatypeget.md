---
title: "IDataFileHeader.RootPropDataTypeGet"
description: "Determines the data type of a data set property from a TDM header file."
---

# IDataFileHeader.RootPropDataTypeGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropDataTypeGet for DataFileHeader

Determines the data type of a data set property from a TDM header file.

## Signature

```python
iRootPropDataTypeGet = Object.RootPropDataTypeGet(PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyRootPropDataType = oMyDataFileHeader.RootPropDataTypeGet("Description")
print (oMyRootPropDataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropDataTypeGet_IDataFileHeader.htm`*
