---
title: "IExcelSheet.Index"
description: "Specifies the position of the worksheet in the workbook."
---

# IExcelSheet.Index

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Index for Sheet

Specifies the position of the worksheet in the workbook.

## Signature

```python
obj.Index
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Workbook.Sheets.Count + 1):
    oCurrSheet = Workbook.Sheets(i)
    oNewGroup = Root.ChannelGroups.Add(oCurrSheet.Name)
    NewGroup.Properties.Add("Description", "Sheet"&oCurrSheet.Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Index_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
