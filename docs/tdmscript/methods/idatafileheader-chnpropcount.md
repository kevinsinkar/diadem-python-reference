---
title: "IDataFileHeader.ChnPropCount"
description: "Determines the number of properties and custom properties of a channel from a TDM header file."
---

# IDataFileHeader.ChnPropCount

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropCount for DataFileHeader

Determines the number of properties and custom properties of a channel from a TDM header file.

## Signature

```python
iChnPropCount = Object.ChnPropCount(ChannelNumber)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyChnPropCount = oMyDataFileHeader.ChnPropCount("[1]/[2]")
print (oMyChnPropCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropCount_IDataFileHeader.htm`*
