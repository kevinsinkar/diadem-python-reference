---
title: "IRepD2ShapeObjFilledAreaSettingsInt.Line"
description: "Specifies the properties of the curve line in the Filled area display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjFilledAreaSettingsInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DFilledAreaSettings

Specifies the properties of the curve line in the Filled area display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMySettings.FillEffects.Pattern = dd.eFillPatternFilled
oMySettings.FillEffects.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD2ShapeObjFilledAreaSettingsInt.htm`*
