---
title: "IDataFileHeader.ChnPropDel"
description: "Deletes a channel custom property from a TDM header file."
---

# IDataFileHeader.ChnPropDel

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropDel for DataFileHeader

Deletes a channel custom property from a TDM header file.

## Signature

```python
obj.ChnPropDel(ChannelNumber, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyDataFileHeader.ChnPropDel("[1]/[1]","test")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropDel_IDataFileHeader.htm`*
