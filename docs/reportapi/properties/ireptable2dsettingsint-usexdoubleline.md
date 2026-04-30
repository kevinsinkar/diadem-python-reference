---
title: "IRepTable2DSettingsInt.UseXDoubleLine"
description: "Specifies whether DIAdem REPORT separates the first row of the 2D table with a thicker horizontal line. You must assign the value TRUE to the property Visible f"
---

# IRepTable2DSettingsInt.UseXDoubleLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseXDoubleLine for 2DTableSettings

Specifies whether DIAdem REPORT separates the first row of the 2D table with a thicker horizontal line. You must assign the value TRUE to the property Visible for 2DTableGridLine in order to use the UseXDoubleLine property.

## Signature

```python
obj.UseXDoubleLine
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
oMySettings.UseXDoubleLine = True
oMySettings.UseYDoubleLine = False
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

*Source: `ReportApi/properties/Report_property_UseXDoubleLine_IRepTable2DSettingsInt.htm`*
