---
title: "IExcelSheet.Index"
description: "Specifies the position of the worksheet in the workbook."
---

# IExcelSheet.Index

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Index for Sheet

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

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
