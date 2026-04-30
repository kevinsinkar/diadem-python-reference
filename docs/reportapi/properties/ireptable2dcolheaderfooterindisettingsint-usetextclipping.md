---
title: "IRepTable2DColHeaderFooterIndiSettingsInt.UseTextClipping"
description: "Specifies whether DIAdem REPORT truncates text at the cell boundary in a 2D table when using individual headers and footers. The property is only valid if you a"
---

# IRepTable2DColHeaderFooterIndiSettingsInt.UseTextClipping

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseTextClipping for 2DTableColumnHeaderFooterIndividualSettings

Specifies whether DIAdem REPORT truncates text at the cell boundary in a 2D table when using individual headers and footers. The property is only valid if you assign the value True to the Enable for 2DTableColumnHeaderIndividualSettings property. You must assign the value False to the UseAutoFontSize property because DIAdem REPORT otherwise adjusts the font size of the text to the size of the cell.

## Signature

```python
obj.UseTextClipping
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To find the <span class="Monospace">UseTextClipping</span> property on the DIAdem REPORT interface, double-click a 2D table and then the tabs <strong>Headers and Footers</strong> and <strong>Text Parameters for Headers</strong> or <strong>Text Parameters for Footers</strong>. Disable the setting <strong>Automatically specify font size for all headings</strong>. The <strong>Text control</strong> list contains the following values:<br attr="ext"/>- <span class="Monospace">No length restrictions</span>: Assigns the value <span class="Monospace">True</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">False</span> to the <span class="Monospace">UseTextClipping</span> property. If texts are wider than a column, DIAdem displays them across the column bounds.<br attr="ext"/>- <span class="Monospace">Truncate at cell border</span>: Assigns the value <span class="Monospace">False</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">True</span> to the <span class="Monospace">UseTextClipping</span> property. DIAdem only displays the part of the text in a cell which fits into this column and truncates the rest on the left and on the right.<br attr="ext"/>- <span class="Monospace">Wrap and Truncate</span>: Assigns the value <span class="Monospace">True</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">True</span> to the <span class="Monospace">UseTextClipping</span> property. DIAdem wraps text which does not fit into a cell and continues the text in the next row.</td></tr></table>
</div>

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyHeaderSettings = oMy2DTable.Settings.Header
oMyHeaderSettings.UseAutoFontSize = False
oMyHeaderSettings.Font.Size = 3
oMyHeaderSettings.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMyColumn1.Settings.RelativeColumnWidth = 10
Col2HeadSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadSettings.Enable = True
Col2HeadSettings.UseTextClipping = False
Col2HeadSettings.UseWordWrap = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseTextClipping_IRepTable2DColHeaderFooterIndiSettingsInt.htm`*
