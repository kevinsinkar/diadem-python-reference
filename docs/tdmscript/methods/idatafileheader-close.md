---
title: "IDataFileHeader.Close"
description: "Closes a TDM header file."
---

# IDataFileHeader.Close

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: Close for DataFileHeader

Closes a TDM header file.

## Signature

```python
obj.Close(WriteChanges)
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyDataFileHeader.ChnPropValSet("[1]/1","Description","Test")
oMyDataFileHeader.close(True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_Close_IDataFileHeader.htm`*
