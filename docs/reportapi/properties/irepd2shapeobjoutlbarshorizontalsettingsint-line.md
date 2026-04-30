---
title: "IRepD2ShapeObjOutlBarsHorizontalSettingsInt.Line"
description: "Specifies the properties of the curve line in the Horizontal outlined bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjOutlBarsHorizontalSettingsInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DOutlineBarsHorizontalSettings

Specifies the properties of the curve line in the Horizontal outlined bars display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.Line.Width = dd.eLineWidth0200
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD2ShapeObjOutlBarsHorizontalSettingsInt.htm`*
