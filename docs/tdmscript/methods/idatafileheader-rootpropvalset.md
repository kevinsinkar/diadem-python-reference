---
title: "IDataFileHeader.RootPropValSet"
description: "Sets the value of a data set property in a TDM header file."
---

# IDataFileHeader.RootPropValSet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropValSet for DataFileHeader

Sets the value of a data set property in a TDM header file.

## Signature

```python
obj.RootPropValSet(PropertyName, PropertyValue)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyDataFileHeader.RootPropValSet("Description","Test")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropValSet_IDataFileHeader.htm`*
