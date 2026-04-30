---
title: "IExcelFileIO.WorkbookInfo"
description: "Returns the WorkbookInfo object that contains information about the workbook that the DataPlugin is currently processing."
---

# IExcelFileIO.WorkbookInfo

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: WorkbookInfo for Workbook

Returns the WorkbookInfo object that contains information about the workbook that the DataPlugin is currently processing.

## Signature

```python
return_value = obj.WorkbookInfo
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyWb = Workbook.WorkbookInfo
Root.Properties.Add("Title", oMyWb.Title)
Root.Properties.Add("Author", oMyWb.Author)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_WorkbookInfo_IExcelFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
