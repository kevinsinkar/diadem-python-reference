---
title: "IRepD2ShapeObjBarsHorizontalSettingsInt.BorderLine"
description: "Specifies the properties of a bar in a 2D axis system in the Horizontal bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsHorizontalSettingsInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for 2DBarsHorizontalSettings

Specifies the properties of a bar in a 2D axis system in the Horizontal bars display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[2]"
oMyShape.YChannel.Reference = "[6]/[1]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BorderLine_IRepD2ShapeObjBarsHorizontalSettingsInt.htm`*
