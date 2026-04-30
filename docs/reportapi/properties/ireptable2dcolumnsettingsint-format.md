---
title: "IRepTable2DColumnSettingsInt.Format"
description: "Specifies the Format definition of the values in a 2D table column in DIAdem REPORT."
---

# IRepTable2DColumnSettingsInt.Format

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Format for 2DTableColumnSettings

Specifies the Format definition of the values in a 2D table column in DIAdem REPORT.

## Signature

```python
obj.Format
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = dd.eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Format_IRepTable2DColumnSettingsInt.htm`*
