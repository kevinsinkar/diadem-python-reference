---
title: "IExcelFileIO"
description: "The Workbook object provides a workbook and the associated properties."
---

# IExcelFileIO

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Workbook

The Workbook object provides a workbook and the associated properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("Title", Workbook.WorkbookInfo.Title)
Root.Properties.Add("Author",Workbook.WorkbookInfo.Author)

oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(2,1)

for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(1,i)
    oNewChannel = oCellBlock.Channels.Add(Name)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iexcelfileio-fileinfo/">FileInfo</a> | <a href="../../properties/iexcelfileio-formatter/">Formatter</a> | <a href="../../properties/iexcelfileio-sheets/">Sheets</a> | <a href="../../properties/iexcelfileio-workbookinfo/">WorkbookInfo</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idataplugin/">DataPlugin</a>.<a href="../../methods/idataplugin-openspreadsheet/">OpenSpreadsheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IExcelFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
