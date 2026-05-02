---
title: "IDataFileHeader.ChnPropExist"
description: "Determines from a TDM header file whether a channel property exists."
---

# IDataFileHeader.ChnPropExist

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropExist for DataFileHeader

Determines from a TDM header file whether a channel property exists.

## Signature

```python
bChnPropExist = Object.ChnPropExist(ChannelNumber, PropertyName)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm" ,"TDM", False)
if oMyDataFileHeader.ChnPropExist("[1]/[1]","Test") :
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

*Source: `TDMScript/methods/TDM_method_ChnPropExist_IDataFileHeader.htm`*
