---
title: "IDataFileHeader.ChnPropIsFixed"
description: "Determines from a TDM header file whether a channel property is a TDM property or a custom property."
---

# IDataFileHeader.ChnPropIsFixed

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropIsFixed for DataFileHeader

Determines from a TDM header file whether a channel property is a TDM property or a custom property.

## Signature

```python
bChnPropIsFixed = Object.ChnPropIsFixed(ChannelNumber, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.ChnPropIsFixed("[1]/[1]","Description") :
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

*Source: `TDMScript/methods/TDM_method_ChnPropIsFixed_IDataFileHeader.htm`*
