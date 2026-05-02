---
title: "IExcelSheet"
description: "The Sheet object provides a worksheet from the open work folder and the associated properties."
---

# IExcelSheet

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Sheet

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The Sheet object provides a worksheet from the open work folder and the associated properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets.Item(1)
Root.ChannelGroups.Add(oCurrSheet.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iexcelsheet-index/">Index</a> | <a href="../../properties/iexcelsheet-maxposition/">MaxPosition</a> | <a href="../../properties/iexcelsheet-minposition/">MinPosition</a> | <a href="../../properties/iexcelsheet-name/">Name</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iexcelsheet-find/">Find</a> | <a href="../../methods/iexcelsheet-getcellblock/">GetCellBlock</a> | <a href="../../methods/iexcelsheet-getcelltype/">GetCellType</a> | <a href="../../methods/iexcelsheet-getcellvalue/">GetCellValue</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/sheets/">Sheets</a>.<a href="../../methods/iexcelsheets-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
