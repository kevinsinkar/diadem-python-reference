---
title: "IDataFileHeader.Save"
description: "Saves changes in a TDM header file."
---

# IDataFileHeader.Save

!!! abstract "Method &middot; `TDMScript.chm`"
    Method: Save for DataFileHeader

Saves changes in a TDM header file.

## Signature

```python
obj.Save
```

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
oMyDataFileHeader.RootPropValSet("Description","Test")
oMyDataFileHeader.Save()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p></div>
</div>

---

*Source: `TDMScript/methods/TDM_method_Save_IDataFileHeader.htm`*
