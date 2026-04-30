---
title: "IRepTable2DColumnSettingsInt.RelativeColumnWidth"
description: "Specifies in DIAdem REPORT the width of a column of the 2D table in relation to the other table columns. For horizontal tables, specifies the height of a table "
---

# IRepTable2DColumnSettingsInt.RelativeColumnWidth

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativeColumnWidth for 2DTableColumnSettings

Specifies in DIAdem REPORT the width of a column of the 2D table in relation to the other table columns. For horizontal tables, specifies the height of a table row of the 2D table in relation to the other rows in the table.

## Signature

```python
obj.RelativeColumnWidth
```

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DTable.Settings.Header.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMyColumn2.Settings.RelativeColumnWidth = 2
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativeColumnWidth_IRepTable2DColumnSettingsInt.htm`*
