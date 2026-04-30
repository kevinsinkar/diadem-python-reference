---
title: "IDataFileHeader.ChnPropDataTypeGet"
description: "Determines the data type of a channel property from a TDM header file."
---

# IDataFileHeader.ChnPropDataTypeGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropDataTypeGet for DataFileHeader

Determines the data type of a channel property from a TDM header file.

## Signature

```python
iChnPropDataTypeGet = Object.ChnPropDataTypeGet(ChannelNumber, PropertyName)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyChnPropDataType = oMyDataFileHeader.ChnPropDataTypeGet("[1]/[1]","Description")
print (oMyChnPropDataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropDataTypeGet_IDataFileHeader.htm`*
