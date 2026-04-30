---
title: "IDataFileHeader.RootPropExist"
description: "Determines from a TDM header file whether a root property exists."
---

# IDataFileHeader.RootPropExist

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: RootPropExist for DataFileHeader

Determines from a TDM header file whether a root property exists.

## Signature

```python
bRootPropExist = Object.RootPropExist(PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.RootPropExist("Test") :
    print ("Exists")
else:
    print() ("Doesn't exist")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_RootPropExist_IDataFileHeader.htm`*
