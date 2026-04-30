---
title: "IRepTable2DColumnSettingsInt.UseTextClipping"
description: "Specifies whether DIAdem REPORT truncates a column of a 2D table at the boundary of the column. You must assign the value False to the UseAutoFontSize property "
---

# IRepTable2DColumnSettingsInt.UseTextClipping

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseTextClipping for 2DTableColumnSettings

Specifies whether DIAdem REPORT truncates a column of a 2D table at the boundary of the column. You must assign the value False to the UseAutoFontSize property because DIAdem REPORT otherwise adjusts the font size of the text to the size of the cell.

## Signature

```python
obj.UseTextClipping
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong> Double-click a 2D table and then the tabs <strong>Column Properties</strong> and <strong>Text Parameters</strong> in order to find the <span class="Monospace">UseWordWrap</span> property on the DIAdem REPORT interface. Disable the setting <strong>Specify font size for all columns automatically</strong>. The <strong>Text control</strong> list contains the following values:<br attr="ext"/>-<span class="Monospace">No length restrictions</span>: Assigns the value <span class="Monospace">True</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">False</span> to the <span class="Monospace">UseTextClipping</span> property. If texts are wider than a column, DIAdem displays them across the column bounds.<br attr="ext"/>-<span class="Monospace">Truncate at cell bound</span>: Assigns the value <span class="Monospace">False</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">True</span> to the <span class="Monospace">UseTextClipping</span> property. DIAdem only displays the part of the text in a cell which fits into this column and truncates the rest on the left and on the right.<br attr="ext"/>-<span class="Monospace">Wrap and truncate</span>: Assigns the value <span class="Monospace">True</span> to the <span class="Monospace">UseWordWrap</span> property and the value <span class="Monospace">True</span> to the <span class="Monospace">UseTextClipping</span> property. DIAdem wraps text which does not fit into a cell and continues the text in the next row.</td></tr></table>
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
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyColumn1.Settings.RelativeColumnWidth = 10
oMyColumn1.TextList(1).Text  = "Very very very very very long text"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Settings.RelativeColumnWidth = 90
oMyColumn2.Channel.Reference = "[1]/[2]"
oMyCol1Settings = oMyColumn1.Settings
oMyCol1Settings.Alignment = dd.eTableAlignmentCentric
oMyCol1Settings.UseWordWrap = True
oMyCol1Settings.UseTextClipping = True
oMyTableSettings = oMy2DTable.Settings
oMyTableSettings.UseAutoFontSize = False
oMyColumn1.Settings.Font.Size = 4.2
oMy2DTable.Columns(2).Settings.Font.Size = 4.2
oMyIndexSettings = oMy2DTable.Settings.IndexSettings
oMyIndexSettings.IndexBegin = 1
oMyIndexSettings.IndexEnd = 3
oMyIndexSettings.IndexIncrement = 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseTextClipping_IRepTable2DColumnSettingsInt.htm`*
