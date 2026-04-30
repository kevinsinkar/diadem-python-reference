---
title: "IDataFileHeader.RootPropCount"
description: "Determines the number of data set properties in a TDM header file."
---

# IDataFileHeader.RootPropCount

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropCount for DataFileHeader

Determines the number of data set properties in a TDM header file.

## Signature

```python
iRootPropCount = Object.RootPropCount
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyRootPropCount = oMyDataFileHeader.RootPropCount
print (oMyRootPropCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropCount_IDataFileHeader.htm`*
