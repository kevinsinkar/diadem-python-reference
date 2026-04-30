---
title: "IRepTable2DIndexSettingsInt.RowHeight"
description: "Specifies the line heights or column heights as a percentage of the worksheet height in a 2D table in DIAdem REPORT. You must assign the value e2DTableIndexMode"
---

# IRepTable2DIndexSettingsInt.RowHeight

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RowHeight for 2DTableIndexSettings

Specifies the line heights or column heights as a percentage of the worksheet height in a 2D table in DIAdem REPORT. You must assign the value e2DTableIndexModeAutomaticallyIncreasing to the IndexMode property in order to use the RowHeight property.

## Signature

```python
obj.RowHeight
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
oMyColumn.Channel.Reference = "[1]/[1]"
oMyIndexSettings = oMy2DTable.Settings.IndexSettings
oMyIndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticallyIncreasing
oMyIndexSettings.RowHeight = 39
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RowHeight_IRepTable2DIndexSettingsInt.htm`*
