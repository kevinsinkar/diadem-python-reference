---
title: "IDataFileHeader.ChnPropValGet"
description: "Determines the value of a channel property from a TDM header file."
---

# IDataFileHeader.ChnPropValGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropValGet for DataFileHeader

Determines the value of a channel property from a TDM header file.

## Signature

```python
vChnPropValGet = Object.ChnPropValGet(ChannelNumber, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyChnPropVal = oMyDataFileHeader.ChnPropValGet("[1]/1", "Description")
print (oMyChnPropVal)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropValGet_IDataFileHeader.htm`*
