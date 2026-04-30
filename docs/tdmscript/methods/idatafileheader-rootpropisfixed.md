---
title: "IDataFileHeader.RootPropIsFixed"
description: "Determines from a TDM header file whether a data set property is a TDM property or a custom property."
---

# IDataFileHeader.RootPropIsFixed

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropIsFixed for DataFileHeader

Determines from a TDM header file whether a data set property is a TDM property or a custom property.

## Signature

```python
bRootPropIsFixed = Object.RootPropIsFixed(PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.RootPropIsFixed("Description") :
    print ("TDM Property")
else:
    print ("Custom Property")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropIsFixed_IDataFileHeader.htm`*
