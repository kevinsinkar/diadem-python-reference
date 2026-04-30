---
title: "IRepTable2DSettingsInt.UseYDoubleLine"
description: "Specifies whether DIAdem REPORT separates the first column of a 2D table with a thicker vertical line. You must assign the value TRUE to the property Visible fo"
---

# IRepTable2DSettingsInt.UseYDoubleLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseYDoubleLine for 2DTableSettings

Specifies whether DIAdem REPORT separates the first column of a 2D table with a thicker vertical line. You must assign the value TRUE to the property Visible for 2DTableGridLine in order to use the UseYDoubleLine property.

## Signature

```python
obj.UseYDoubleLine
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
oMySettings = oMy2DTable.Settings
oMySettings.GridHorizontal.Visible = True
oMySettings.GridVertical.Visible = True
oMySettings.UseXDoubleLine = False
oMySettings.UseYDoubleLine = True
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseYDoubleLine_IRepTable2DSettingsInt.htm`*
