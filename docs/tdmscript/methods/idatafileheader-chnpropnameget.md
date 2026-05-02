---
title: "IDataFileHeader.ChnPropNameGet"
description: "Determines the name of a channel property from a TDM header file."
---

# IDataFileHeader.ChnPropNameGet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropNameGet for DataFileHeader

Determines the name of a channel property from a TDM header file.

## Signature

```python
sChnPropNameGet = Object.ChnPropNameGet(ChannelNumber, ChnPropIndex)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
oMyChnPropName = oMyDataFileHeader.ChnPropNameGet("1/1",2)
print (oMyChnPropName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropNameGet_IDataFileHeader.htm`*
