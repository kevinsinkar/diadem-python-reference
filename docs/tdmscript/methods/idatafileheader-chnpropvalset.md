---
title: "IDataFileHeader.ChnPropValSet"
description: "Sets the value of a channel property in a TDM header file."
---

# IDataFileHeader.ChnPropValSet

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: ChnPropValSet for DataFileHeader

Sets the value of a channel property in a TDM header file.

## Signature

```python
obj.ChnPropValSet(ChannelNumber, PropertyName, PropertyValue)
```

## Python example

```python
oMyDataFileHeader = DataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyDataFileHeader.ChnPropValSet("[1]/1","Description","Test")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_ChnPropValSet_IDataFileHeader.htm`*
