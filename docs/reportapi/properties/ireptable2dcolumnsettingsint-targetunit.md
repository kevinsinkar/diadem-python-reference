---
title: "IRepTable2DColumnSettingsInt.TargetUnit"
description: "Specifies the unit for a column in a 2D table. If you assign a value to the property TargetUnit, DIAdem converts the channels you want to display into this unit"
---

# IRepTable2DColumnSettingsInt.TargetUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TargetUnit for 2DTableColumnSettings

Specifies the unit for a column in a 2D table. If you assign a value to the property TargetUnit, DIAdem converts the channels you want to display into this unit. If DIAdem cannot convert the unit, DIAdem does not display the data.

## Signature

```python
obj.TargetUnit
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
oMyColumn.Settings.TargetUnit = "min"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TargetUnit_IRepTable2DColumnSettingsInt.htm`*
