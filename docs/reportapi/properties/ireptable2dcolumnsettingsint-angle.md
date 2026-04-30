---
title: "IRepTable2DColumnSettingsInt.Angle"
description: "Specifies the text angle of the column entries in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnSettingsInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for 2DTableColumnSettings

Specifies the text angle of the column entries in a 2D table in DIAdem REPORT.

## Signature

```python
obj.Angle
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngle0` | 0 |  |
| `eAngle090` | 1 | 90 |
| `eAngle180` | 2 | 180 |
| `eAngle270` | 3 | 270 |

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
oMyColumn.Settings.Angle = dd.eAngle090
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepTable2DColumnSettingsInt.htm`*
