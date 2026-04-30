---
title: "IExcelSheet"
description: "The Sheet object provides a worksheet from the open work folder and the associated properties."
---

# IExcelSheet

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Sheet

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
